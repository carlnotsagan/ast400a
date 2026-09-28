# Homework 2

_AST400A - Theoretical Astrophysics - Fall 2025, Steward Observatory_

**Due Tue. Oct. 14, 12:30p (before class)**

-

Relevant Chapters: [HKT](https://arizona-ua.primo.exlibrisgroup.com/permalink/01UA_INST/1ffcblk/alma991048844104203843) Ch. 4,5; Pols Lectures Ch. 3,5 [here](https://www.astro.ru.nl/~onnop/education/stev_utrecht_notes/chapter1-4.pdf). LeBlanc Chapters 5,6. Not a complete list of the topics covered in the problem set. You are encouraged to work together on the problem sets but you must submit your own work. 

**Submitting your work:** You are encouraged to work in groups, but your final solutions should be your own work! Turn into D2L as a PDF. In most cases, solutions will be found by hand, then written up in LaTeX/Markdown/Word and exported as a final PDF. If you have not worked with LaTeX before consider starting from one of the Overleaf Homework Templates [here](https://tr.overleaf.com/gallery/tagged/homework).

**Extra credit:** HW assignments submitted that were prepared using LaTeX will earn 10 points extra credit. If you used LaTeX to prepare your solutions, make a note of this in D2L textbox.

**Total: (150 points)** 

--

1. **Total: (30 points)** - The [Planck](https://en.wikipedia.org/wiki/Planck%27s_law) function 

    * (**a**) - Show that $
\frac{dB_{\nu}}{dT} = \frac{2 k_{\rm{B}}^3 T^2}{h^2 c^2} \left [ \frac{x^4 e^x}{(e^x-1)^2} \right ]~.$ (**10 points**)

    * (**b**) - Compute the maximum of the bracketed term using derivatives. This will require a numerical solution. (**10 points**)
    * (**c**) - Plug the maximum back into your variable substitution to compute the favored photon energy. In a few sentences compare your result to that from Pols 5.24 and what this suggests for the Rosseland mean opacity. (**10 points**)


2. **Total: (35 points)** - Assume a star of radius $R_\star$ having a density profile equal to 
$\rho( r)=\rho_{c} \left ( 1 - \frac{r}{R_\star} \right )$ and a nuclear production rate per unit mass equal to $\epsilon( r) = \epsilon_{c} \left (1 - \frac{r}{0.2 R_\star} \right ) \ \  \textrm{for} \ r~\leq 0.2~R_\star$ and $\epsilon( r) = 0 \ \  \textrm{for} \ r~\gt 0.2~R_\star~.$
    * (**a**) - Compute the luminosity of the star at its surface in terms $R_\star$, $\rho_{c},$ and $\epsilon_{c}$ **(15 points)** 
    * (**b**) - Plug in present day solar values, you can use HKT 9.2.3, and compute a numerical value for the luminosity. **(10 points)**
    * (**c**) - Compute the nuclear timescale for this star and compare it to the nuclear timescale of the Sun. **(10 points)** 
_For this problem, you may solve by hand or using [SymPy](https://www.sympy.org/en/index.html). If using sympy, upload the PDF output of your notebook as part of the solution._
3. **Total: (20 points)** - Assume that 10 eV of energy per atom found in the Sun is emitted during some chemical reaction taking place. Also assume that the Sun is composed of pure hydrogen. 
    * (**a**) - Calculate the total energy emitted by this chemical process ($E_{\rm{chem}}$). **(5 points)**
    * (**b**) - Compute the nuclear timescale for this star assuming a solar luminosity. **(5 points)**
    * (**c**) - In a few sentences describe if it is then possible that the energy source of the Sun is chemical in nature? Why or why not? **(10 points)**

4. **Total: (25 points)** - Conceptual questions from Pols Chapter 3. Respond in a few sentences.
    * (**a**) - What do we mean by local thermodynamic equilibrium (LTE)? Why is this a good assumption for stellar interiors? What is the difference between LTE and thermal equilibrium (as treated in Ch. 2)? **(10 points)**
    * (**b**) - In what type of stars does degeneracy become important? Is it important in main-sequence stars? Is it more important in high mass or low mass MS stars? **(5 points)**
    * (**c**) - Explain qualitatively why for degenerate matter, the pressure increases with the density. **(5 points)**
    * (**d**) - In the central region of a star we find free electrons and ions. Why do the electrons become degenerate first? Why do the ions never become degenerate in practice? **(5 points)**

5. **Total: (40 points)** - Produce a stellar model using MESA-Web [here](http://user.astro.wisc.edu/~townsend/static.php?ref=mesa-web-submit) of initial mass between 0.5 $M_{\odot}$ to 30 $M_{\odot}$. **Set your stopping condition to central hydrogen mass fraction lower limit of 1e-6**. We will focus on the evolution of the star to the end of the main-sequence. 
<br>
**Note**: If you have issues for your choice of mass, change to a lower initial mass, the defaults are set for a 1 $M_{\odot}$ model to evolve to a white dwarf. 
<br> 
 **Extra Credit**: If you download and install MESA (instructions [here](https://docs.mesastar.org/en/latest/installation.html)) to your laptop or on UA HPC (account creation info [here](https://hpcdocs.hpc.arizona.edu/registration_and_access/account_creation/#overview)) then produce a model using one of the MESA [_Test Suites_](https://docs.mesastar.org/en/latest/test_suite.html) you can earn 25 points extra credit. 

    * (**a**) - Produce a _profile_ plot of $\nabla_{\rm{ad}}$ and $\nabla_{\rm{rad}}$ as a function of mass ($m/M_{\odot}$) or radius ($r/R_{\odot}$) during the main-sequence (or elsewhere if using a `test_suite`) and _label_ where the star is **convective** and **radiative**. **(15 points)**
    * (**b**) - Produce an HRD using the history data from your model and label the `main-sequence`. On the same plot, plot the present location of the Sun. **(15 points)**
    * (**c**) - Produce a time-evolution plot of the luminosity of the `pp` and `cno` burning categories and determine which is the dominant burning category for your model. If there is a crossover point, identify the approximate central $T_6$ this occurs at. **(10 points)**
