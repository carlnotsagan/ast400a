# Homework 2

_AST400A - Theoretical Astrophysics - Fall 2026, Steward Observatory_

**Due Fri. Oct. 9, 11:59pm (End of day)**

-

Relevant Chapters: [HKT](https://arizona-ua.primo.exlibrisgroup.com/permalink/01UA_INST/1ffcblk/alma991048844104203843) Ch. 4,5; Pols Lectures Ch. 3,5 [here](https://www.astro.ru.nl/~onnop/education/stev_utrecht_notes/chapter1-4.pdf). LeBlanc Chapters 5,6. Not a complete list of the topics covered in the problem set. You are encouraged to work together on the problem sets but you must submit your own work. 

**Submitting your work:** You are encouraged to work in groups, but your final solutions should be your own work! Turn into D2L as a PDF. In most cases, solutions will be found by hand, then written up in LaTeX/Markdown/Word and exported as a final PDF. If you have not worked with LaTeX before consider starting from one of the Overleaf Homework Templates [here](https://tr.overleaf.com/gallery/tagged/homework).

**Extra credit:** HW assignments submitted that were prepared using LaTeX will earn 10 points extra credit. If you used LaTeX to prepare your solutions, make a note of this in D2L textbox.

**Total: (150 points)** 

--

1. **Total: (30 points)** - **<span style="color:#762fef">My Favorite Photons</span>** 
>_For this problem, you may solve by using [SymPy root solve](https://docs.sympy.org/latest/guides/solving/find-roots-polynomial.html) or similar tool._
    * (**a**) - Show that the [Planck](https://en.wikipedia.org/wiki/Planck%27s_law) function  $
\frac{dB_{\nu}}{dT} = \frac{2 k_{\rm{B}}^3 T^2}{h^2 c^2} \left [ \frac{x^4 e^x}{(e^x-1)^2} \right ]~.$ (**10 points**)

    * (**b**) - Compute the maximum of the bracketed term using derivatives. This will require a numerical solution. (**10 points**)
    * (**c**) - Plug the maximum back into your variable substitution to compute the favored photon energy. In a few sentences compare your result to that from Pols 5.24 and what this suggests for the Rosseland mean opacity. (**10 points**)


2. **Total: (35 points)** - **<span style="color:#a8a62b">On the Burning Away</span>** - Assume a star of radius $R_\star$ having a density profile equal to 
$\rho( r)=\rho_{c} \left ( 1 - \frac{r}{R_\star} \right )$ and a nuclear production rate per unit mass equal to $\epsilon( r) = \epsilon_{c} \left (1 - \frac{r}{0.2 R_\star} \right ) \ \  \textrm{for} \ r~\leq 0.2~R_\star$ and $\epsilon( r) = 0 \ \  \textrm{for} \ r~\gt 0.2~R_\star~.$
>_For this problem, you may solve by hand or using [SymPy](https://www.sympy.org/en/index.html). If using sympy, upload the PDF output of your notebook as part of the solution._
    * (**a**) - Compute the luminosity of the star at its surface in terms $R_\star$, $\rho_{c},$ and $\epsilon_{c}$ **(15 points)** 
    * (**b**) - Plug in present day solar values, you can use HKT 9.2.3, and compute a numerical value for the luminosity. **(10 points)**
    * (**c**) - Compute the nuclear timescale for this star and compare it to the nuclear timescale of the Sun. **(10 points)** 
3. **Total: (15 points)** - **<span style="color:#eda412">I've Got Sunshineee, On a Cloudy Day</span>** - Assume that 10 eV of energy per atom found in the Sun is emitted during some chemical reaction taking place. Also assume that the Sun is composed of pure hydrogen. 
    * (**a**) - Calculate the total energy emitted by this chemical process ($E_{\rm{chem}}$). **(5 points)**
    * (**b**) - Compute the nuclear timescale for this star assuming a solar luminosity. **(5 points)**
    * (**c**) - In a few sentences describe if it is then possible that the energy source of the Sun is chemical in nature? Why or why not? **(5 points)**

4. **Total: (15 points)** - **<span style="color:#fc0c1c">Fire Burn and Cauldron Bubble</span>** - Conceptual questions from [Pols Chapter 5](https://www.astro.ru.nl/~onnop/education/stev_utrecht_notes/chapter5-6.pdf). Respond in a sentence or two. 

    * (**a**) - Why does convection lead to a net heat flux upwards, even though there is no net mass flux (upwards and downwards bubbles carry equal amounts of mass)? **(5 points)**
    * (**b**) - Explain the Schwarzschild criterion in simple physical terms (using Archimedes law) by drawing a schematic picture . Consider both cases $\nabla_{\rm{rad}} \gt \nabla_{\rm{ad}}$ and $\nabla_{\rm{rad}} \lt \nabla_{\rm{ad}}$ . Which case leads to convection? **(5 points)**
    * (**c**) - What is meant by the superadiabaticity of a convective region? How is it related to the convective energy flux (qualitatively)? Why is it very small in the interior of a star, but can be large near the surface? **(5 points)**

5. **Total: (45 points)** - **<span style="color:#009E60">Starz2therainbow</span>** - Produce a stellar model using [`MESA-Web`](http://user.astro.wisc.edu/~townsend/static.php?ref=mesa-web-submit) of initial mass between 0.5 $M_{\odot}$ to 30 $M_{\odot}$ with stopping condition to central $^{1}\rm{H}$ mass fraction lower limit of $10^{-6}$. 
>**Note**: If you have issues for your choice of mass, change to a lower initial mass, the defaults are set for a 1 $M_{\odot}$ model to evolve to a white dwarf.
**Extra Credit**: If you download and install MESA (instructions [here](https://docs.mesastar.org/en/latest/installation.html)) to your laptop or on UA HPC (account creation info [here](https://hpcdocs.hpc.arizona.edu/registration_and_access/account_creation/#overview)) then produce a model using one of the MESA [_Test Suites_](https://docs.mesastar.org/en/latest/test_suite.html) you can earn 25 points extra credit. 
    * (**a**) - **Produce** a [_profile_](https://docs.mesastar.org/en/latest/using_mesa/output.html#) plot of $\nabla_{\rm{ad}}$ and $\nabla_{\rm{rad}}$ as a function of mass ($m/M_{\odot}$) or radius ($r/R_{\odot}$) during the main-sequence (or elsewhere if using a `test_suite`) and _label_ where the star is **convective** and **radiative**. **(10 points)**
        * (**a1**) - **Describe** how you determined where the star was **convective** and **radiative**. **(5 points)**
    * (**b**) - **Produce** a time-evolution plot of the luminosity of the `pp` and `cno` burning categories and determine which is the dominant burning category for your model.  **(10 points)**
        * (**b1**) - **Describe** when the particular category dominates the burning and why. **(5 points)**
    * (**c**) - **Produce** a central $T-\rho$ plot using the history data from your model and use it to describe the **dominant source of opacity in the core**, and in the **envelope (below the surface)**. **(10 points)**
        * (**c1**) - **Describe** how the dominant opacity sources were determined. **(5 points)**
