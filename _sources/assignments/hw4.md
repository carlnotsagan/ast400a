# Homework 4 (Optional)

_AST400A - Theoretical Astrophysics - Fall 2025, Steward Observatory_

**Due Tue. Dec. 9, 12:30p (before class)**

-

Chapters: [HKT](https://arizona-ua.primo.exlibrisgroup.com/permalink/01UA_INST/1ffcblk/alma991048844104203843) Ch. 2; Pols Lectures Ch. 9,12 [here](https://www.astro.ru.nl/~onnop/education/stev_utrecht_notes/chapter1-4.pdf). Not a complete list of the topics covered in the problem set. 

**Submitting your work:** You are encouraged to work in groups, but your final solutions should be your own work! Turn into D2L as a PDF. In most cases, solutions will be found by hand, then written up in LaTeX/Markdown/Word and exported as a final PDF. If you have not worked with LaTeX before consider starting from one of the Overleaf Homework Templates [here](https://tr.overleaf.com/gallery/tagged/homework).

**Extra credit:** HW assignments submitted that were prepared using LaTeX will earn 5 points extra credit. If you used LaTeX to prepare your solutions, make a note of this in D2L textbox.

**Total: (150 points)** - Only will replace your lowest HW grade if this grade is higher. 

--


1. **Total: (50 points)** - **Core Collapse** - Assume the collapse of a 1.2$M_{\odot}$  core from an initial density of $\rho_{i}=10^{9} \ (\rm{g \ cm}^{-3})$ to a final density $\rho_{f}=10^{15} \ (\rm{g \ cm}^{-3})$.
    * (**a**) - Compute the gravitational potential energy released in the collapse. **(20 points)** 
    * (**b**) - Compute the total energy released by the Sun $\tau_{\rm{MS}}\sim10^{10} \ (\rm{yr})$ and $L=L_{\odot}=\rm{constant}$. **(10 points)**
    * (**c**) - Compute the timescale for core-collapse using $\rho_{i}$ and the dynamical timescale $\tau_{\rm{dyn}}=1/2(G\rho)^{-1/2}$. **(10 points)**
    * (**d**) - In a few sentences, qualitatively compare the two energy values computed and the difference in timescales, as well as briefly explain where all the energy goes for the core-collapse case. **(10 points)** 

    
2. **Total: (40 points)** - **Observational Properties of Massive Stars** - Consider the mass loss prescription for hot O and B stars from ([Vink et al. 2000](https://ui.adsabs.harvard.edu/abs/2000A&A...362..295V/abstract)):
$$
\textrm{log} \left ( \frac{\dot{M}}{M_{\odot}\rm{yr}^{-1}} \right ) = -6.7 + 2.2 \ \textrm{log} \left ( \frac{L}{10^{5}L_{\odot}} \right)  - 1.3 \  \textrm{log}\left ( \frac{M}{30M_{\odot}} \right) - 1.2~\textrm{log}\left ( \frac{v_{\infty}/v_{\rm{esc}}}{2.0} \right )~, 
$$
and the approximate main-sequence lifetime of

$$
t_{\rm{MS}}\approx 10^{10} \left ( \frac{M}{M_{\odot}} \right )^{-2.9}~(\rm{yrs})
$$

 * (**a**) - Compute the $\textbf{mass loss rate}$ $\dot{M}$ for a $40M_{\odot}$ star with a luminosity of $L=5.62\times10^{5}L_{\odot}$ and assuming a ratio of $v_{\infty}/v_{\rm{esc}}=2.6$. **(10 points)** 
 * (**b**) - Compute the approximate **main-sequence lifetime** for this star. **(5 points)**
 * (**c**) - Assuming the mass-loss is the constant value you found in **(a)** during the main-sequence, and that the star initially has a H-rich envelope that is 30% of its total mass, compute how much **mass of the H-rich envelope** remains at the terminal-age main sequence. **(15 points)**
 * (**d**) - Based on the above result, **describe** if this star will likely become a red supergiant or not include at least one reason that you came to this conclusion. **(10 points)**
 

3. **Total: (30 points)** - **Early stages of evolution and the mainsequence phase** - Conceptual questions from Pols Chapter 9. Respond in a few sentences.
    * (**a**) - What is the Hayashi line? Why is it a line, in other words: why is there a whole range of possible luminosities for a star of a certain mass on the HL? **(10 points)**
    * (**b**) - Why do no stars exist with a temperature cooler than that of the HL? What happens if a star would cross over to the cool side of the HL? **(10 points)**
    * (**c**) - Why is there a mass-luminosity relation for ZAMS stars? (In other words, why is there a unique luminosity for a star of a certain mass?) **(5 points)**
    * (**d**) - What determines the shape of the ZAMS is the HR diagram? **(5 points)**

    
    
4. **Total: (30 points)** - **Wolf-Rayet Stars** - Produce a stellar model using MESA-Web [here](http://user.astro.wisc.edu/~townsend/static.php?ref=mesa-web-submit) of initial mass between 40 $M_{\odot}$ to 100 $M_{\odot}$. **Keep your stopping condition to iron core collapse (default)** - We will try to at least evolve the model to He-dep. Sometimes a non-UA email works better.
<br>
**Note**: If you have issues for your choice of mass, change to a different initial mass. 
<br> 
 **Extra Credit**: If you download and install MESA (instructions [here](https://docs.mesastar.org/en/latest/installation.html)) to your laptop or on UA HPC (account creation info [here](https://hpcdocs.hpc.arizona.edu/registration_and_access/account_creation/#overview)) then produce a model using one of the MESA [_Test Suites_](https://docs.mesastar.org/en/latest/test_suite.html) you can earn 10 points extra credit. 

    * (**a**) - Produce an HR diagram of the model as a scatter plot, but color the data according to the log of the absolute value of the mass loss rate value at a given HR data pair and label the following **(10 points)**: 
        *  **Label**: _Main-Sequence_, _Hertzsprung Gap_, _RGB (if applicable)_ **(5 points)**
        *  **Label**: a vertical line of log effective temperature where the star becomes a WR **or** RSG star and label that region. **(5 points)**
    * (**b**) - In a few sentences, describe which information is needed to determine the WR subclass this model corresponds to at the end of the simulation (or earlier) and how you could conclude this. **(5 points)**
    * (**c**) - In a few sentences, discuss the likely evolutionary fate of this stellar model based on its final mass, He/CO core mass, and envelope mass and if it will leave a stellar remnant behind. **(5 points)**
        
