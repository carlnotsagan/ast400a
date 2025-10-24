# Homework 3

_AST400A - Theoretical Astrophysics - Fall 2025, Steward Observatory_

**Due Tue. Nov. 4, 12:30p (before class)**

-

Relevant Chapters: [HKT](https://arizona-ua.primo.exlibrisgroup.com/permalink/01UA_INST/1ffcblk/alma991048844104203843) Ch. 5; Pols Lectures Ch. 10,11,12 [here](https://www.astro.ru.nl/~onnop/education/stev_utrecht_notes/chapter1-4.pdf). LeBlanc Chapters 2,6. Not a complete list of the topics covered in the problem set. 

**Submitting your work:** You are encouraged to work in groups, but your final solutions should be your own work! Turn into D2L as a PDF. In most cases, solutions will be found by hand, then written up in LaTeX/Markdown/Word and exported as a final PDF. If you have not worked with LaTeX before consider starting from one of the Overleaf Homework Templates [here](https://tr.overleaf.com/gallery/tagged/homework).

**Extra credit:** HW assignments submitted that were prepared using LaTeX will earn 5 points extra credit. If you used LaTeX to prepare your solutions, make a note of this in D2L textbox.

**Total: (150 points)** 

--


1. **Total: (50 points)** - Assuming that while on the Horizontal Branch, the Sun will burn helium via the triple-$\alpha$ reaction only and that the luminosity in the core will be constant $L_{\rm{HB}}=100L_{\odot}$.
    * (**a**) - Compute the energy emitted by the triple-$\alpha$ reaction in MeV. **(10 points)** 
    * (**b**) - Compute the fraction $f$ of mass transformed into energy for the triple-$\alpha$ reaction. **(10 points)**
        * _Hint: [Mass–energy equivalence](https://en.wikipedia.org/wiki/Mass%E2%80%93energy_equivalence)_
    * (**c**) - Compute the total emitted energy on the horizontal branch assuming 10% of the total mass ($1M_{\odot}$) will be converted to ${^{12}\rm{C}}$ and with the efficiency found in (**b**). **(10 points)**
    * (**d**) - Compute the total time this star will spend on the horizontal branch ($t_{\rm{HB}}$). **(10 points)** 
    * (**e**) - Compare this to the typical main-sequence lifetime for a Solar like star and describe physically why the $t_{\rm{HB}}$ is shorter or longer. **(10 points)**

2. **Total: (25 points)** - Consider a homogeneous spherical cloud with temperature $T$ and density $\rho$. Neglecting all factors except for gravitational and thermal energy, it may be assumed that the cloud can collapse under the condition: $-\Omega>2U$. 
    * (**a**) - Calculate the Jeans length $R_{\rm{J}}$ for this cloud, the length at which this condition is met. **(15 points)**
    * (**b**) - Respond in a few sentences: If a cloud has a radius larger than its $R_{\rm{J}}$, will it collapse? What are the next steps of a cloud that has began to collapse? **(10 points)**
 

3. **Total: (30 points)** - Conceptual questions from Pols Chapter 10,12. Respond in a few sentences.
    * (**a**) - Why does the luminosity of a star increase on the main sequence? Why do low-mass stars, likethe Sun, expand less during the main sequence than higher-mass stars? **(10 points)**
    * (**b**) - Explain what happens during the ‘hook’ at the end of the main sequence of stars more massivethan the Sun. **(5 points)**
    * (**c**) - Explain the existence of a Hertzsprung gap in the HRD for high-mass stars. Why is there noHertzsprung gap for low-mass stars? **(10 points)**
    * (**d**) - Explain why the timescales of the burning stages from C-burning onward are very short comparedto the H- and He-burning phases. **(5 points)**

    
    
4. **Total: (45 points)** - Produce a stellar model using MESA-Web [here](http://user.astro.wisc.edu/~townsend/static.php?ref=mesa-web-submit) of initial mass between 0.5 $M_{\odot}$ to 30 $M_{\odot}$. **Set your stopping condition to central helium mass fraction lower limit of 1e-6**. Sometimes a non-UA email works better.
<br>
**Note**: If you have issues for your choice of mass, change to a different initial mass. 
<br> 
 **Extra Credit**: If you download and install MESA (instructions [here](https://docs.mesastar.org/en/latest/installation.html)) to your laptop or on UA HPC (account creation info [here](https://hpcdocs.hpc.arizona.edu/registration_and_access/account_creation/#overview)) then produce a model using one of the MESA [_Test Suites_](https://docs.mesastar.org/en/latest/test_suite.html) you can earn 15 points extra credit. 

    * (**a**) - Produce a _profile_ plot of $\nabla_{\rm{ad}}$ and $\nabla_{\rm{rad}}$ as a function of mass ($m/M_{\odot}$) or radius ($r/R_{\odot}$) during core-helium burning phase (or elsewhere if using a `test_suite`) and 
        * _label_ where the star is **convective** and **radiative**. **(15 points)**
        * _describe_ the expected evolutionary fate of the star and your reasoning. **(5 points)**
    * (**b**) - Produce an HR diagram using the history data from your model and label at least **four** of the applicable evolutionary phases:
        *  _Main-Sequence_, _Red Giant Branch_, _Asymptotic Giant Branch_, _Blue Loop_, _Hertzsprung Gap_ **(15 points)**
    * (**c**) - Produce a time-evolution (`model_number` or `star_age` for example) plot of the luminosity of the all helium burning $L_{\rm{He}}$ and use this to show if the star undergoes a _helium flash_ or not. 
        * Describe in a few words your reasoning based on the results of the plot. **(10 points)**
