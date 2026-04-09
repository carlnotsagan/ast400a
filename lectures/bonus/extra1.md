---
marp: true
theme: gaia
class: invert
style: |
  video::-webkit-media-controls {
    will-change: transform;
  }
---



<!-- _class: title -->
<!--_color: lightgreen-->

![bg ](https://apod.nasa.gov/apod/image/2509/IrasDisk_Webb_2045.jpg)


# AST/PTYS 545 - Astrophysics of Stars and Planets - Spring 2026, Steward Observatory

<br>
<br>

## Prof. Carl Fields


<style scoped>
p { text-align: right; }
</style>

<br>

<small>_IRAS 04302: Butterfly Disk Planet Formation_
Image Credit & Copyright: [NASA, ESA, CSA, Webb](https://www.nasa.gov/) 
</small>

---

### Exoplanet Detection, Characterization, and Statistics 

<small>_Notes from Handbook of Exoplanets: [Transit Photometry as an Exoplanet Discovery Method](https://link.springer.com/rwe/10.1007/978-3-319-30648-3_117-1), [Stellar Limb Darkening’s Effects on Exoplanet Characterization](https://link.springer.com/rwe/10.1007/978-3-319-55333-7_41), Review: [Exoplanet Statistics and Theoretical Implications](https://www.annualreviews.org/content/journals/10.1146/annurev-astro-112420-020055)._</small>

#### **April, 10, 2026** Agenda:
* Lecture **(20m)**
* ICA - XXX **(20m)**
* Report out on ICA  - **Due: EoD Today to D2L? (5m)**
---

<!-- header: 'AST545A' -->

<!-- paginate: true -->



### Exoplanets, Brown Dwarfs, and Stars

<img src="https://github.com/carlnotsagan/ast545sp25/blob/main/lectures/week5/mass_cuts.jpg?raw=true"  
width="500"
img align="right" />

Fate of stars in various mass classes. Credit: [HKT Fig. 2.4].

* **Stars** - Undergo nuclear fusion of H. 

* **Brown Dwarfs** 
  * Not massive enough to fuse H to He, $M\lesssim0.085M_{\odot}$. 
  * Deuterium ($^{2}\rm{H}$ or $\rm{D}$) can burn at $T\approx10^{6} (\rm{K})$. 

* **Planets** - No $^{1}\rm{H}$ or $^{2}\rm{H}$ fusion and at a mass range of $M\lesssim0.05M_{\odot}$.


---

### Planet Formation Overview

_More details in [Handbook of Exoplanets by Phil Armitage](https://link.springer.com/referenceworkentry/10.1007/978-3-319-55333-7_135)._

Planet formation can described by a _bottom up_ theory: 
  * planetary systems form within largely gaseous protoplanetary disks from initially microscopic solid material. 
  * Different physical processes dominate as growth proceeds.

See for example _On the Formation of Planetesimals Via Secular Gravitational Instabilities with Turbulent Stirring_ [(Youdin 2011)](https://ui.adsabs.harvard.edu/abs/2011ApJ...731...99Y/abstract)

---

### Planet Formation Overview

* 1. Early Phases (particle sizes of $s$ of $\mu$m to m) - primarily aerodynamic and material physics. 

* 2. Gravitational forces become increasingly important 
  * first between growing planetesimals ($s \geq \rm{km}$) and 
  * later between protoplanets and gas in the disk (for masses $M \geq 0.1M_{\oplus}$, where $M_{\oplus}$ is the mass of the Earth).

* 3. Giant planet growth from 3 to 20 + $M_{\oplus}$ cores is limited initially by the ability of their gaseous envelopes to cool and subsequently by how fast the surrounding disk can supply mass.

---


### Transit Photometry as an Exoplanet Discovery Method

<img src="https://github.com/carlnotsagan/ast545sp25/blob/main/lectures/week5/exoplanet_discoveries.webp?raw=true"  
width="550"
img align="right" />

Fractions by which various detection methods contributed to the accumulated sample of known planets are shown, for years since 1995-2018.

* By 2018, 78% of all known planets had been discovered by transits. 

---


### Fundamentals of the Transit Method

As the planet passes in front of the star, its. flux diminishes by a fractional denoted as $\Delta F$. 

Assumpting of negligible flux from the planet and of spherical shapes of the star and planet, $\Delta F$ is given by the ratio of the areas of the planet and the star:

$$
\Delta F \approx \left ( \frac{ R_{\rm{planet}} }{R_{\rm{star}}} \right )^{2} = k^2
$$

where $k$ is the radius ratio.

---

### Fundamentals of the Transit Method

**$t_{{T}}$** - total duration of the transit event
**$t_{{F}}$** - the time of totality, in which the entire planet disk is in front of the stellar disk, 

This allows us to define the impact parameter (minimal projected distance to the center of the stellar disk during the transit):


$$
b = \frac{a}{R_{\rm{star}}} \textup{cos}~i \equiv \left ( \frac{(1-k)^2 - [ \rm{sin}^{2} (\pi t_{\rm{F}}/P) / \rm{sin}^{2} (\pi t_{\rm{T}}/P)](1+k)^2}{ \rm{cos}^{2} (\pi t_{\rm{F}}/P) / \rm{cos}^{2} (\pi t_{\rm{T}}/P) } \right )^{1/2}
$$


where we have $a$ is the orbital semimajor axis, $i$ the orbital inclination, and $P$ the orbital period.

---

### Fundamentals of the Transit Method

Using photometric data alone we can define the scale of the system or the ratio between the semimajor axis and the radius of the star,

$$
\frac{a}{R_{\rm{star}}} = \frac{1}{\sqrt{\rm{tan}(\pi t_{\rm{T}}/P)}} \sqrt{(1+k)^2 - b^2}
$$

combining with Kepler's laws allows us to make an estimate of the mean density of the star,

$$
\rho_{\rm{star}} = \frac{3 \pi}{GP^2} \left ( \frac{a}{R_{\rm{star}}} \right )^3
$$

---

### Fundamentals of the Transit Method

<img src="https://github.com/carlnotsagan/ast545sp25/blob/main/lectures/week5/transit.jpg?raw=true"  
width="550"
img align="right" />

**Detection Probability**

Estimate given in [Winn 2010](https://arxiv.org/abs/1001.2010)

$
p_{\rm{tra}} = \left(\frac{R_{s} \pm R_{p}}{a} \right) \left(\frac{1 + e~\rm{sin ~\omega}}{1-e^2} \right)
$.

* a typical Hot Jupiter with a semimajor axis of 0.05 AU, $p\sim10\%$, 
* while for an earth-like planet at 1 AU from a solar-like star, $p\sim0.5\%$. 


---

### Transmission Spectroscopy
<small>_See this Chapter from [Handbook of Exoplanets](https://link.springer.com/rwe/10.1007/978-3-319-30648-3_100-2) for recent overview including discoveries with _JWST_._</small>

<img src="https://github.com/carlnotsagan/ast545sp25/blob/main/lectures/week5/atmosphere_example.jpg?raw=true"  
width="650"
img align="right" />

Key aspect of this method is that the planet’s transit depth ($\delta$) is _**wavelength dependent**_.

Illustration of transit and eclipse geometry and the atmospheric scale height $H$. **Credit: Robinson 2017**.

---

### Transmission Spectroscopy
<img src="https://github.com/carlnotsagan/ast545sp25/blob/main/lectures/week5/depth.jpg?raw=true"  
width="550"
img align="right" />

* At wavelengths where the atmosphere is more opaque due to absorption by atoms or molecules, the planet blocks slightly more stellar flux.

Example Transit light curve measured with the Hubble Space Telescope for the hot Jupiter WASP-12b from Kreidberg et al. 2015.


---

### Transmission Spectroscopy

<img src="https://github.com/carlnotsagan/ast545sp25/blob/main/lectures/week5/spectrum.jpg?raw=true"  
width="550"
img align="right" />

* To measure these variations, 
  * the light curve is binned in wavelength, and 
  * the light curve from each channel is fit separately with a transit model. 


The measured transit depths as a function of wavelength constitute the _transmission spectrum_.

---

### Transmission Spectroscopy

<img src="https://github.com/carlnotsagan/ast545sp25/blob/main/lectures/week5/spectrum.jpg?raw=true"  
width="550"
img align="right" />

The measured transit depths as a function of wavelength constitute the _transmission spectrum_.

Example near-infrared transmission spectrum of the hot Jupiter WASP-43b, which has a strong water! absorption feature centered at 1.4 $\mu\rm{m}$.

---

### Transmission Spectroscopy

* Theoretical models of the atmosphere require radiative transfer simulations, but we can make an order of magnitude estimate.

* The amplitude of spectral features in transmission is then 

$$
\delta_{\lambda} = \frac{ (R_{\rm{planet}} + nH)^2 }{ R^2_{\rm{star}} } - \frac{ R_{\rm{planet}}^2 }{ R_{\rm{star}}^2 } \approx 2n R_{\rm{planet}} H / R^2_{\rm{star}}
$$


But even for these ideal cases, the amplitude of spectral features is just $\delta_{\lambda} ∼ 0.1\%$. For Earthlike planets, the expected amplitude is **two to three orders of magnitude smaller**, depending on host star size.

---
 
### Limb Darkening

<img src="https://media.springernature.com/full/springer-static/image/chp%3A10.1007%2F978-3-319-55333-7_41/MediaObjects/395338_1_En_41_Fig1_HTML.jpg?as=webp"  
width="500"
img align="right" />

* Stars are not uniformly illuminated light sources. 
* The surface brightness distribution can be modified by 
  * dark stellar spots, bright faculae, plages, flares, and the presence of the stellar atmosphere. 
  
_In dwarf stars this means that we see apparently darker regions to the apparent limb than in the apparent center of the star._

---

### Limb Darkening

The result can an introduce curvature to the transit light curve and can also modify the transit depth up to 50%.

<img src="https://github.com/carlnotsagan/ast545sp25/blob/main/lectures/week5/limb_darkening.jpg?raw=true"  
width="550"
img align="right" />

_Example_: Transits of the same exoplanet around the same star, only the limb darkening treatment has been changed. 

There are many models and parameters for limb darkening models that **require comparison to observations**. 

---

### Defining and Interpreting Planet Occurrence Rate

The intrinsic **occurrence rate** (or the often interchangeably used term, frequency) of planets.

We can define this occurance rate as ("the frequency of planets"):


$$
\boxed{\bar{n_{p}} = \frac{\textrm{Total \# of planets}}{\textrm{Total \# of stars}}}
$$

this rate is the easiest to measure but requires the planets be resticted to a particular plane and assumptions about the host star and possible companions. 

---

### Defining and Interpreting Planet Occurrence Rate

In this defintion we define the ("the frequency of planetary systems")

$$
\boxed{F_{p} = \frac{\textrm{Total \# of planetary systems}}{\textrm{Total \# of stars}}}
$$

The ratio of these quantities gives the (_average planet multiplicity_): 

$$
\boxed{\bar{m_{p}} = \frac{\bar{n_{p}}}{F_{p}} \frac{\textrm{Total \# of planets}}{\textrm{Total \# of planetary systems}}}
$$

---

### Defining and Interpreting Planet Occurrence Rate


<img src="https://github.com/carlnotsagan/ast545sp25/blob/main/lectures/week11/exop_mult.png?raw=true"  
width="550"
img align="right" />


In practice, we find that $\bar{m_{p}}$ is very model / theoretically dependent, and $F_{p}$ often requires many assumptions about the system. 


The close-in ($P$ < 400 days) _Kepler_ planets in the period–radius plane. The radius valley at $\sim2 R_{\oplus}$ (see [Section 2.1.4](https://arxiv.org/pdf/2103.02127)) is visible. Credit: [Zhu & Dong 2021](https://www.annualreviews.org/content/journals/10.1146/annurev-astro-112420-020055#abstract_content).

---

### Planet Distribution in the Period–Radius Plane


### Hot Jupiters

* Planets with $8 R_{\oplus} < R_{p} < 20 R_{\oplus}$ and $P<10$ days. 

* **Occurance Rates** - Transit surveys statistics suggest $\bar{n}_{p}\sim0.62\%$ where as RV studies typically report rates twice this value. 

* **Multiplicity** - Only 1/49 in the above graphic show hot Jupiters with small close companions. Data suggest about $2\%$ have nearby ($P\lt20$ days, small $\sim1-4  R_{\oplus}$), and $\sim$ coplanar companions. 

The low multiplicity rate of hot Jupiters supports the general idea that most of them have undergone some **large-scale migrations**.

---

### Hot Neptune desert

* The region $2 R_{\oplus} < R_{p} < 8 R_{\oplus}$ and $P<2-4$ days is described as the Hot Neptune (or sub-Jovian) desert.

* **Occurance Rates** - $0.61 \pm 0.07\%$ for the planet frequencies $\bar{n}_{p}$.

* **Multiplicity** - $\sim 23\%$ of these systems have a companion.

Theories describing the triangle like boundaries include effects of photoevaporation and tidal effects. More massive planets can be circularized more efficiently without tidal effects.  

---

### Ultra-short-period planets (USPs)

* Planets with of $0.5-2.0R_{\oplus}$ and $P<1$ day.

* **Occurance Rates** - $\bar{n}_{p}=0.38\%$ planet frequencies 
* **Multiplicity** - $\sim20\%$ - but likely higher since USPs can be more misaligned relative to their outer companions. 

It has been suggested that these were not formed in-situ, partially due to the comparable rates to hot Jupiters. Multiple theories for this have been proposed including that they are the surviving cores of tidally disrupted hot Jupiters ([Jackson et al 2013](https://iopscience.iop.org/article/10.1088/0004-637X/779/2/165)).

---

### Radius valley

Region of $R_{p}\approx 2.0 R_{\oplus}$ and periods of $3 < P < 30$ days.

Theories for this bifurcation is **atmospheric evaporation driven by high-energy photons** from the host star (photoevaporation).

* Under this assumption: planets with core masses of a few Earth masses, the high-energy radiation is sufficient to unbind the entire hydrogen/helium atmosphere if its initial mass fraction is below some critical value. 

_The radius valley thus emerges, separating planets with and without extended atmospheres_. See more recently ([Burn et al 2024](https://www.nature.com/articles/s41550-023-02183-7)).

---


# In-Class Assignment

**In class**: Work on ICA [here](https://carlnotsagan.github.io/ast400a/assignments/extra1.html) with **groups** per usual. Discuss conceptual questions together and prepare answers to share at the end of class.

* Choose someone that will report out the groups responses ahead of time!

**After Class: Due: End of the Day to D2L**

**Note:** _The goal of ICAs are to use plots produced in the notebook for discussion and interpretation of results presented in lecture in groups **and** as a class._



