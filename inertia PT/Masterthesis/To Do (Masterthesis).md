# Important guidline to fokus on
- <span style="font-size:120%;color:red">Don't touch the box algo anymore!</span>
- <span style="font-size:120%;color:red">determine the Phase transition point</span>
	- use the latest data I have ⟹ of half avg and max avg
- <span style="font-size:120%;color:red">determine $\nu$ with the derivative of $\mathcal{B}$</span>
- [ ] Browser Uni aufräumen
- clean the proposal
- sort the introduction and theorie
- explain the algorithm at it's current state and it's flaws and also the ways to refine it
- [ ] clean the folder **sqaureboxEvaluation**
- make / clear snapshots with plots with the latest algo. ==am Windows PC==
	- **new folder**
	- **clear naming**
	- **neat** / **oversee-able**
	- 112k
		- [x] avg max
			<!-- - [ ] 0.06 -->
			- [x] 0.065
			<!-- - [ ] 0.067 -->
			<!-- - [ ] 0.0675 -->
			- [x] 0.068
			<!-- - [ ] 0.069 -->
			- [x] 0.07
		- [x] avg half
			<!-- - [ ] 0.06 -->
			- [ ] 0.065
			<!-- - [ ] 0.067 -->
			<!-- - [ ] 0.0675 -->
			- [ ] 0.068
			<!-- - [ ] 0.069 -->
			- [ ] 0.07
	- 28k
		- [x] avg max
			<!-- - [ ] 0.06 -->
			- [ ] 0.065
			<!-- - [ ] 0.067 -->
			<!-- - [ ] 0.0675 -->
			- [ ] 0.068
			<!-- - [ ] 0.069 -->
			- [ ] 0.07
		- [x] avg half
			<!-- - [ ] 0.06 -->
			- [ ] 0.065
			<!-- - [ ] 0.067 -->
			<!-- - [ ] 0.0675 -->
			- [ ] 0.068
			<!-- - [ ] 0.069 -->
			- [ ] 0.07
	- 7k
		- [x] avg max
			<!-- - [ ] 0.06 -->
			- [ ]  0.065 
			<!-- - [ ] 0.067 -->
			<!-- - [ ] 0.0675 -->
			- [ ] 0.068
			<!-- - [ ] 0.069 -->
			- [ ] 0.07
		- [x] avg half
			<!-- - [ ] 0.06 -->
			- [ ] 0.065
			<!-- - [ ] 0.067 -->
			<!-- - [ ] 0.0675 -->
			- [ ] 0.068
			<!-- - [ ] 0.069 -->
			- [ ] 0.07
	- Density distribution **exemplarisch** anhand von 112k für 
		- [ ] 0.065
		- [ ] 0.068
		- [ ] 0.07
- [x]  <span style="font-size:120%;color:orange">write down the scaling formula for the order parameter</span>
	- <span style="font-size:120%;color:orange">determine $\beta$</span>
- [ ] git checkout to the ***last*** **phase-peak-pit-height-tune-algo**
- [ ] compare the box placement for stdDev and halfstdDev
- [ ] evaluate binder for 28k particles with halfstddev and compare the plot with stdDev
	
# Box Algo
- [ ] put the box evaluation on the cluster and evaluate the data there
- [ ] ask kayro for rights to push to upstream
## peak pit width tuning
- [x] did a new strange branch... from phase-peak tune...
- [x] need to branch it...
- did a combination of height and width mul variation in combination with an alternation in varying this value. Also increased the reduction of the width to get less loop breaks / faster results
- changed bins from 500 ⟹ 600
- [ ] the best result for placing the squares would be to average only over the peaks in the standard deviation range of the highest peak (part of the other branch)
## Evaluate 
- [x] reeval at 224k seed 05000 m 0.067
- [x] Save the box size of the evaluated boxes

## finite-size-scaling_phase-peak-pit-height-tune-algo 
new branch ⟹ fss_ppphta_ebox-fit-in-pp
- [ ] ==clean the code from old unused stuff== delete old code
	- [x] ==make a backup before cleaning==
	- [ ] filter_same_pits
	- [x] remove commented code in finite_size_scaling
	- [ ] remove keep_pbc in the middle
	- [ ] remove dist_pbc
	- [ ] substitute pbc everywhere
	- [ ] remove commented code from  `evaluate`
	- [ ] move the auxiliary functions out of the main code...
- [x] quality management with correct distance measurement
- [ ] filter_same_pits
	- [ ] check if distance between pits is wide enough that the evaluation box fits in
	      ![[Pasted image 20251024224645.png]]
	    It should lead to that in too "narrow" phases no evaluation squares are placed. But it does not provide that the box is complete inside the phase and also does not prevent overlapping with evaluation boxes in dilute phases, if they are placed at the boarder of a rectangle box.
	    Overlapping is only prevented, when the square is placed in the middle of a rectangle box.
- [ ] ==problem:== evaluating the particle number of split eval boxes ( those which overlap over the mainbox border)  ⟹ particles at vertical border between the left and the right split box are counted twice atm!
	- [x]  ⤷ Don't split squares in `subbox_to_square_withpeak_dilute_dense_new` split only, when  creating the plotting rectangles.
	- [ ] adjust `box_to_rectangle` / `box_to_rectangle_list` <span style="color:red"> needs another name ==not== rectangle</span>
	- [ ] adjust sorboxes ⟸ because there are no lists of squareboxes anymore
- [ ] add a dilute vs dense eval boxes counter to quality management

# Jupyter 
- [ ] test new code / cleaned code, after square_box split was moved to  box_to_rectangle
- [ ] compare the densities / particle numbers of squarebox split and not split
- [ ] **Dict to csv**
    ```python
    import csv  
    
    cars = [     {"Brand": "Toyota", "Model": "Corolla", "Year": 2020},     {"Brand": "Honda", "Model": "Civic", "Year": 2019},     {"Brand": "Ford", "Model": "Focus", "Year": 2018} ]  
    
    # CSV file name 
    csv_filename = "cars.csv" 
    
     # Define the field names (headers) 
     fieldnames = ["Brand", "Model", "Year"]  
     
     # Writing to CSV 
     with open(csv_filename, mode='w', newline='') as file:   
			     writer = csv.DictWriter(file, fieldnames=fieldnames)
			     writer.writeheader()  # Write header row    
			     writer.writerows(cars)  # Write data rows   
        ```
- [ ] https://pandas.pydata.org/docs/reference/api/pandas.read_csv.html
	- [ ] https://pandas.pydata.org/docs/reference/api/pandas.unique.html
- [x] sort determine CP
# Evaluate
## Determine CP
linear approximation optimization with aritras interpolation method
- [x] Read Aritras Code and ask if something isn't clear
	- [x] "data_phase_transition_with_errors.csv" ⟹ how did he get the errors
	- [x] what are **unique L values** ⟹ a designated system size 
	      With the method `.unique()`you can filter rows for certain values.
	- [ ] Udl ⟹ is the Bindercumlant of mean largest cluster length $d_l$: $\mathcal{B}(d_l)$
	      In my case $d_l$ is $\rho$ of the evaluation boxes: $\mathcal{B}(\rho_\text{box})$
	- [ ] Udl_se means? ⟹ I guess it is the error
	- [x] What does `from scipy.interpolate import splrep, splev`?
		- [ ] splrep(_x_, _y_, _w=None_, _xb=None_, _xe=None_, _k=3_, _task=0_, _s=None_, _t=None_, _full_output=0_, _per=0_, _quiet=1_)[[source]](https://github.com/scipy/scipy/blob/v1.16.2/scipy/interpolate/_fitpack_py.py#L164-L305)
		      Find the B-spline representation of a 1-D curve.
		- [ ] splev(_x_, _tck_, _der=0_, _ext=0_)[[source]](https://github.com/scipy/scipy/blob/v1.16.2/scipy/interpolate/_fitpack_py.py#L308-L395)
		      Evaluate a B-spline or its derivatives.
	- [x] why `{py} subset_df = data_frame[data_frame['L'] == L_value]`
	      `{py} subset_df['Udl']` picks a column of a csv file
	- [ ] `{py} result = minimize(lambda params: objective(params, curves_data, curves_se_data), initial_guess, method='BFGS')` 
		- [ ] <u>BFGS</u> Minimization of scalar function of one or more variables using the BFGS algorithm.
		       https://docs.scipy.org/doc/scipy/reference/optimize.minimize-bfgs.html#optimize-minimize-bfgs
		       
		    n numerical optimization, the Broyden–Fletcher–Goldfarb–Shanno (BFGS) algorithm is **an iterative method for solving unconstrained nonlinear optimization problems**. Like the related Davidon–Fletcher–Powell method, BFGS determines the descent direction by preconditioning the gradient with curvature information.
		       https://en.wikipedia.org/wiki/Broyden%E2%80%93Fletcher%E2%80%93Goldfarb%E2%80%93Shanno_algorithm
Evaluate a B-spline or its derivatives.
`{cpp} printf("\nHello World!")`
Find the B-spline representation of a 1-D curve.
- [x] how do I export dicts to csv files
- [x] Export the data from
	- [x] binder_max_avg_dicts
	- [x]  binder_half_avg_dicts
	      `omit 3.5k and 7k `
- [ ] apply the optimization⟹decide by the optimization error which box size to choose
- [x] evaluate the derivative of the binder cumulant
## order parameter
- [x] determine order parameter $\rho_\text{dense}-\rho_\text{dilute}$ ==Feng2025==
      ![[Pasted image 20251103233523.png]]
- [ ] plot it
- [ ] write down the scaling function for the orderparameter
- [ ] determine $\beta$
## susceptibility
- [ ] determine the susceptibility $\chi$ ![[Pasted image 20251103233452.png]] $\chi \equiv \left( \frac{L^{3}}{v_{D}} \right) \frac{\Braket{\Delta \phi^{2}}_{L}}{\Braket{\phi}_{L}}$  <br> With $v_{D}\equiv\frac{\pi d^{3}_{hs}}{6}$ the volume of a single particle. With $d_{hs}=2^{1/6}\sigma$ $v_{\text{sphere}}=\frac{4}{3}\pi r^{3}=\frac{4}{3}\pi \left( \frac{d_{hs}}{2} \right)^{3}=\frac{4}{3 \cdot 8} \pi d_{hs}^{3}=\frac{\pi}{6}d_{hs}^{3}$   The susceptibility $\chi$ is maximal at the CP
      ![[Pasted image 20251103235225.png]]
- [ ] translate $\chi$ in $2D$ <br> $\chi \equiv \left( \frac{L^{2}}{v_{D}} \right) \frac{\Braket{\Delta \phi^{2}}_{L}}{\Braket{\phi}_{L}}$   With $v_{D}\equiv\frac{\pi d^{2}_{hs}}{4}$  the volume of a single particle. With $d_{hs}=2^{1/6}\sigma$  <span style="color:red;font-size:100%;">valid?</span> in 2D?<br>
- [ ] get $L$: in my case it is the length of the evaluation box.
	- [ ] need to retrieve it from calculate binder from sub box 
	- [ ] ==take care== $L$ is ==different== for *max* and *half*
	- [ ] create a column $L_{\text{evalbox}}$  
- [ ] plot $\chi$
- [ ] determine $\gamma$ 
- [ ] 
$\text{boxRatio}=R=10$
$\text{fillRatio}=\phi=0.5$
$L_{yHalf} = \sqrt{\left( \frac{N\cdot\pi\cdot\sigma^2}{(4\cdot R \cdot \phi)} \right)}/2$
$L_{xHalf} = R\cdot L_{yHalf}$
$\phi = \frac{N \cdot \pi \cdot \sigma^2}{4\cdot R\cdot2\cdot L_{yHalf}^2}$
### box boundaries xlo,xhi,ylo,yhi,zlo,zhi L_y=sqrt(N Pi sigma²/(20 phi))
region 	box block -${LxHalf} ${LxHalf} -${LyHalf} ${LyHalf} -0.5 0.5	
# Simulate
<span style="font-size:120%;color:green"> Atm there is enough simulation data</span>
- [ ] 224k
	- [ ] .04 
		- [x] 5 eq
		- [x] 5 pr
		- [x] 4 eq
		- [x] 4 pr
	- [ ] .045
		- [x] 5 eq
		- [x] 5 pr
		- [x] 4 eq
		- [x] 4 pr
	- [ ] .05 
		- [x] 5 eq
		- [x] 5 pr
		- [x] 4 eq
		- [x] 4 pr
	- [ ] .055 
		- [x] 5 eq
		- [x] 5 pr
		- [x] 4 eq
		- [x] 4 pr
	- [ ] .06 
		- [x] 3 eq
		- [x] 3 pr
	- [ ] .062 
		- [x] 3 eq
		- [x] 3 pr
	- [ ] .064 
		- [x] 3 eq
		- [ ] 3 pr
	- [ ] .065 
		- [x] 3 eq
		- [ ] 3 pr
	- [ ] .0676 
		- [x] 4 eq
		- [ ] 4 pr
		- [x] 5 eq
		- [ ] 5 pr
	- [ ] .0677 
		- [x] 4 eq
		- [ ] 4 pr
		- [x] 5 eq
		- [ ] 5 pr
	- [ ] .0678 
		- [x] 4 eq
		- [ ] 4 pr
		- [x] 5 eq
		- [ ] 5 pr
	- [ ] .0679 
		- [x] 4 eq
		- [ ] 4 pr
		- [x] 5 eq
		- [ ] 5 pr
## Create-sim
- [ ] add some something like a progress bar / time estimation
- [ ] a checker which simulations are finished 
- [ ] a little GUI, where you can see all the data you already have
- [ ] modify it that it does not run on the cluster... it need to connect via sftp to do the stuff... would be better...
- [x] add dependency to create-simulation - dependency of production run to equilibration run
	-  Hier ein Beispiel: 
```{SLURM}
#!/bin/bash
jid1=$(sbatch --parsable impact_sol_${NUM}1.sh)
jid2=$(sbatch --parsable --dependency=afterok:$jid1 impact_sol${NUM}2.sh)
jid3=$(sbatch --parsable --dependency=afterok:$jid2 impact_sol${NUM}_3.sh)
echo "Stage 3 jobs submitted: $jid1 → $jid2 → $jid3"
```

-  Jeder Job wird zugewiesen, z.B. jid1, jid2, ... und der folgende Job muss auf das OK des vorherigen warten, d. h. dass er abgeschlossen ist. Das wird gemacht mit `--dependency=afterok`.
	- There has to be the possibility to set up equilibration and production at the same time where the number of cores for the equilibration run will be divided by 8 (make sure that its an integer)
	- <span style="font-size:200%;color:gold;"> soooo geil dependency funktioniert</span>
- [ ] ask why the equilibration run is still so slow in comparison to the production run by $ts=1^{-4}$ 

# Read
- [ ] Feng2025~Theory for the anomalous phase behavior of inertial active Brownian particles
	- [ ] + Supplement

# Thesis
- [ ] gescheiten Titel überlegen ⟹ criticality/universality of underdamped brownian particles non equilibrium 

# Report
<span style="color:red" > finish the Slides today </span>
- [ ] Slides:
	- [ ] 112k different m: .06, .065, .067, .068, ~~.069~~ ⟹.07
		- [ ] pictures of Δy Density Distribution 
		- [ ] pictures for avg 
		- [x] pictures for peak 
		      <span style="color:gold;font-size:100%;">⟹ the peak evaluation is depreciated for now!</span>
		- [ ] square size max
		- [ ] square size half
- [ ] add the current results for CP and $\nu$ 
- [x] Fitting $\mathcal{B}$ ⟹ CP:
	- [ ] show CP in ledgend
	- [ ] max evalbox size
		- [ ] replot the non cut out plot with legend and higher smoothing
	- [ ] half evalbox size
		- [x] replot non cut out with legend
		- [x] replot cut out with legend
- [x] Fitting $\nu$ 
- [x] Fitting $\beta$
- [x] Fitting $\gamma$ 
- [ ] 

# Test note
- [ ] this is a test note $\sqrt{x}$ 
$$\frac{ \partial f }{ \partial x }
$$
$\partial \Delta$
$\frac{ \partial f }{ \partial 2}$

$x^{2}\frac{ \partial g(x) }{ \partial x }$

```mermaid 
%% --- %%
%% config: %%
 %% layout: elk %%
 %% look: handDrawn %%
 %% theme: dark %%
%% --- %%
flowchart TB
	a[Tenant admins] 
	a-->SubRoles
	
	subgraph SubRoles [Sub Roles]
		direction LR
		b[Playbook admins]
		c[Playbook managers]
		d[Playbook global viewers]
		b-->c
		c-->d
	end
```
# New Note
1. First 
2. Second 
3. $\frac{ \partial y }{ \partial x }$ 
4. $t_{7}$ ❃☩⚔☠✠⤭✼⛥꙳

# MIPS
- competition between the time scale of reorientation and collision
- overdamped ⟹ no reason for bouncing back
- underdamped ⟹ the bounce back
- Reentrance effekt for higher Pe with higher masses 
  ![[Pasted image 20251118121845.png]] (Hecht2021)
- Something (Weaks-chanderler potential) is hard to parallelize 
## Feng(25-04) Theory from the anomalous phase behavior of inertial active Brownian particles
- $\mathcal{S}=\frac{\varepsilon}{\zeta U_{0}\sigma}$ gives us a measure for how much can particles overlap?
- Coexisting phases in non equilibrium systems are the binodals ⟹ when you start in a uniformal regime you don't see the binodal
- in equilibrium you don't have a free energy
- reentrance disappears, when the stiffness $\mathcal{S}$ ? Question from Benno
	- you need both stiffness and inertia?
	- if you dont have inertia
	- They didnt rule out the influence of inertia?
- mechanical balance of the interface - modeled by the *dynamic stress tensor* $\mathbb{\Sigma}$ 
- My questions
	- no contradiction to the groups work?⟹yes
	- where is a parallelization problem?
		- ⟹only for strictly hard spheres 
		- WCA isn't about strict hard spheres than I understood it correct
		- what exactly the identify as the binodal?
			- ⟹ When there are two separated phases
			- but since you don't have a free energy this is speculative / not accurate
- $\text{St}\equiv \frac{\tau_{M}}{\tau_{R}}$, $\tau_{M}\equiv \frac{m}{\zeta}$, $\zeta=\gamma_{t}$, $[\tau_{M}]=s=\frac{kg}{\frac{kg}{s}}$ ⟹$[\gamma_{t}]=\frac{kg}{s}$ <span style="font-size:80%;color:orange;">(assumption that </span>$\tau_M$ <span style="font-size:80%;color:orange;">is a time)</span>
	- $\zeta$ translational drag coefficient  $[\gamma]=1$
	- $\tau_{R}$ represents characteristic reorientation/persistence time (or inverse rotational diffusion) $\tau_{R}=\frac{1}{D_{R}}$, $D_{R}=\frac{k_{B}T_{b}}{\gamma_{r}}$, $[D_{t}]=\frac{m^{2}}{s}$ $[D_{R}]=\frac{1}{s}$ $\gamma_{r,\text{sphere}}=8 \pi \eta R^{3}$, $\eta$ is the dynamic viscosity, $[\eta]=\frac{kg}{m s}$, $[k_{B}]=\frac{J}{K}$ 
	- $St \equiv \tau_{M} \cdot \frac{1}{\tau_{R}} =\frac{m}{\gamma_{t}} \cdot D_{R}= \frac{m}{\gamma_{t}} \cdot \frac{k_{B}T_{b}}{\gamma_{r}}$ , $[St]=kg \cdot \frac{1}{s}$ 
	- What are $\gamma_{t}$ , $\gamma_{r}$ and $T_{b}$ in my case? <span style="color:orange;font-size:100%;">lammps script</span>  
		``` python
# use:: fix ID group-ID langevin/lh Tstart Tstop gamma_t seed alpha(=10*gamma_r/sigma^2/gamma_t) omega <yes/no> zero <yes/no>
fix 	noise all langevin/lh 1.0 1.0 1.0 §seed 10 omega yes zero yes	# add Langevin thermostat (noise+friction)
`````
		``` python
cocompute	erot all erotate/sphere
ththermo_style	custom step temp epair c_erot etotal press
ttthermo		5000
`````
	  ![[Pasted image 20251118151512.png]]
		- $\gamma_{t}=1$
		- $\gamma_{r}$ 
			- Since $\alpha=\frac{10 \gamma_{r}}{\sigma^{2}\gamma_{t}}=10$
			- $\gamma_{r}=1 \cdot \sigma^{2}\gamma_{t}=1$  

# JC
## 25-12-2 Separation of Microscale Chiral Objects by Shear Flow
DOI: 10.1103/PhysRevLett.102.158103
This is old from 2009
![](Pasted%20image%2020251202122408.png)![](Pasted%20image%2020251202122436.png)
- chiral molecules
- switched the gene off of the bacteria for motility (Dennis asked if a ethic commission approved this🤭), the bacteria was also mutated that it does not split, but in stead grow and get a spiral structure (all controled by protein)
- microfluidic channel 
- shear two opposite planes against each other ⟹ shear on microscale chiral objects in between
- bacterias drift perpendicular to the shear plane
- Net drift results from the preferential alignment of helices with streamlines, with a direction that depends on the chirality of the helix and the sign of the shear rate. 
- separation efficiency $\eta = \frac{|N_{L}-N_{R}|}{N_{L}+N_{R}}$  
- The flow around the particle is approximated linear $u(y)=\frac{vy}{H}$ 