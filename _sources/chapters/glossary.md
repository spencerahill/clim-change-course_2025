# Glossary
```{note}
The definitions in this glossary are **working definitions** appropriate for this class: they're what you need to know to follow the material we cover.  

Just be aware that many of the terms have more general, precise, and/or nuanced meanings when used in other contexts of climate science or physics.  Anything in that category can be found in parentheses at the end of a given definition.
```

```{glossary}
absorption
  In radiative transfer, when a photon hits a molecule, exciting the molecule, and gets destroyed in the process.

  To be contrasted with {term}`scattering` (a.k.a. reflection) and {term}`transmission`

absorption band
  In atmospheric radiative transfer, a band of wavelengths where one or more of the greenhouse gases within the atmosphere strongly absorbs electromagnetic radiation.  For example, carbon dioxide strongly absorbs radiation in a band centered at a wavelength of 15 microns.  There are several other important absorption bands coming from carbon dioxide, water vapor, and ozone.

  Within the atmosphere's absorption bands, the {term}`absorptivity` is close to 1, meaning most photons get absorbed.  Outside absorption bands, absorptivity is close to zero, meaning most photons pass through the atmosphere without being absorbed.

absorptivity
  The fraction of electromagnetic radiation at a given wavelength that gets absorbed.   It is a dimensionless quantity and thus unitless.
  
  Identical to the {term}`emissivity` at that wavelength (by [Kirchhoff's law of thermal radiation](https://en.wikipedia.org/wiki/Kirchhoff%27s_law_of_thermal_radiation); see {term}`emissivity` for more.)

adiabatic
  A process in the atmosphere and ocean in which there is no net exchange of heat or mass between an parcel or water parcel and its surroundings.  As such, its energy---for the atmosphere, its {term}`moist static energy` to good enough approximation for us---remains unchanged.

  For an air parcel with {term}`relative humidity` less than 100%, the resulting cooling with height follows the {term}`dry adiabatic lapse rate` of \(\Gamma_\mathrm{d}\equiv g/c_p=9.8\text{ K km}^{-1}\)

aerosol
  A small solid particle in the atmosphere.  There are naturally occuring aerosols such as sea salt and dust.  There are also {term}`anthropogenic` aerosols such as sulfate and smoke from combustion.

  Thir precise radiative properties varies a lot across aerosol species.
  
  With respect to historical emissions of aerosols by humans, overall they have slightly increased the planetary {term}`albedo` by directly {term}`scattering` {term}`shortwave radiation` back to space, which constitutes a negative {term}`radiative forcing`.

  They have contributed an even more negative---but highly uncertain---negative radiative forcing through their influence on cloud {term}`albedo` via their role as cloud condensation nuclei.

albedo
  The fraction of the sun's radiation that is reflected back to space.  It is a dimensionless quantity and thus unitless.  Usually denoted with a Greek lower-case alpha, $\alpha$.
  
  The {term}`planetary albedo` is the global-mean, time-mean value of the albedo at the {term}`top of atmosphere`.

  It turns out that within Earth's climate system there is very little reflection of {term}`longwave radiation`, which is why albedo is only associated with shortwave radiation.

  Technically, albedo is a *spectral* property: the precise albedo of a given material depends on the precise wavelength of the radiation incident on that material, not just the bulk SW vs. LW.  So, formally, $\alpha=\alpha(\lambda)$.  But in the {term}`two-band approximation`, we treat it as being a bulk property of just the {term}`shortwave radiation`.

analytical framework
  One or more equations representing the physical laws of nature that we apply to a particular problem at hand.

  Some examples: To understand {term}`emission temperature`, we use the {term}`planetary energy balance` analytical framework.  To understand the {term}`greenhouse effect`, we use the {term}`one-layer greenhouse model` analytical framework.

  Any analytical framework we will make use of makes some assumptions and approximations.  This is necessary, to boil the given problem down to the simplest possible explanation.
  
  Truly understanding a given analytical framework means not just memorizing the equation(s), or even the physical meaning of each term appearing in the framework, but also being cognizant of those underlying approximations, and under what conditions they could break down.

anthropogenic
  A fancy term for *caused by humans*.  As opposed to *natural*, *naturally occuring*, etc.  
  
  So, for example, we can distinguish between *natural climate changes* on the one hand (as occur, say, between the ice ages and interglacial periods due to the planet's naturally occuring orbital fluctuations), with, on the other hand, *anthropogenic climate change* which is the set of ongoing changes to Earth's climate caused by human activities.

atmosphere
  The gaseous envelope surrounding a planet.  For Earth, this extends roughly 100~km up from the {term}`surface`, is mostly transparent to {term}`shortwave radiation`, but strongly absorbs {term}`longwave radiation` due to the presence of {term}`greenhouse gas` molecules.

  Earth's atmosphere consists of several distinct levels; only the two that are nearest the surface are of our concern: the {term}`troposphere` and {term}`stratosphere`.

blackbody
  A body that emits electromagnetic radiation according to the {term}`Stefan-Boltzmann law`.  The sun and Earth's surface can be approximated as perfect blackbodies, whereas Earth's atmosphere is an imperfect blackbody, meaning it has an {term}`emissivity` that is less than one.

Carnot cycle
  The 4-stage cycle representing the optimal way that an engine can produce mechanical {term}`work`.

  For our purposes, it comes up as a useful theoretical model for understanding {term}`tropical cyclone`s.

  For more: [Wikipedia page](https://en.wikipedia.org/wiki/Carnot_cycle)

Clausius-Clapeyron
  The equation from thermodynamics that gives rise to the roughly exponential increase in saturation specific humidity with warming, at a rate of approximately $7\%\text{ K}^{-1}$.   

  Insofar as the {term}`relative humidity` stays fixed, this 7% increase per Kelvin warming extends to the specific humidity too.  But note that changes in *relative* humidity---or lack thereof---are *not* directly determined by Clausius-Clapeyron.
  
  (More formally, the Clausius-Clapeyron equation specifies the dependence of saturation vapor pressure on temperature: $d\ln e^*/dT=L_v/(R_vT^2)$, where $e^*$ is saturation vapor pressure, $T$ is temperature, $L_v=2.5\times10^6\text{ J kg}^{-1}$ is the latent heat of vaporization, and $R_v=461.5\text{ J kg}^{-1}\text{ K}^{-1}$ is the specific gas constant of water vapor.  Plugging those values of $L_v$ and $R_v$ in and using temperature ranges within the troposphere, so $T\sim200$ to $300\text{ K}$, yields the approximate $7\%\text{ K}^{-1}$ scaling.)

climate model
  A representation of Earth's climate system on a computer, usually a supercomputer.  Traditionally, they work by chunking the ocean, atmosphere, and land into lots of small *gridboxes* (though the shapes aren't always a simple box) and solving the equations of motion, equations of radiative transfer, and equations representing other key processes forward in time.

  The laws of nature and the real Earth are *continuous*, whereas a computer treats things as *discrete*: climate model gridboxes have finite sizes, and the climate model advances forward in time in discrete finite chunks, e.g. 30 minutes per *timestep*.  This creates all sorts of biases and uncertainties.

climate sensitivity
  The global-mean surface temperature change caused by a doubling of atmospheric CO$_2$ concentration.  Units Kelvin or degrees Celsius.  
  
  There are two meaningful variants: {term}`equilibrium climate sensitivity` and {term}`transient climate sensitivity`, which differ based on the *timescale* considered.

  This cannot be directly observed: we don't have a 2nd Earth available where we can instantly double ${\text{CO}_2}$ and then watch equilibrate over thousands of years.  It therefore must be estimated using climate models.

cloud
  You know, those white puffy things in the sky.  Suspensions of liquid water droplets or ice crystals or a mixture of the two.

  Can be categorized in numerous ways.  For our purposes, there are three key cloud types: {term}`low cloud`, {term}`high cloud`, and {term}`cumulonimbus` cloud.

  Hugely important for Earth's {term}`top of atmosphere` radiative balance, i.e. the {term}`planetary energy balance`, due to their high {term}`albedo` for {term}`shortwave radiation` and strong {term}`absorption` of {term}`longwave radiation`.  These are quantified in the {term}`cloud radiative effect`.  
  
  As such, also hugely important for the *change* in Earth's TOA radiative balance in response to a {term}`radiative forcing`, as quantified in the {term}`cloud feedback`.

cloud condensation nuclei
  Particles, a.k.a. {term}`aerosol`, suspended in the atmosphere that water can condense onto to form cloud droplets or ice crystals in air that has reached {term}`saturation`.  Often abbreviated CCN.

  In the absence of sufficient CCN, even once air reaches {term}`saturation`, cloud droplets or ice crystals will not immediately form, and instead the air will be become *supersaturated*.

  All else equal, the more CCN present in a given saturated air parcel, the more cloud droplets and/or ice crystals will form.  For a fixed amount of condensed water, this results in smaller droplets on average, which acts to increase the cloud's {term}`albedo`.

cloud feedback
  The {term}`radiative feedback` due to changes in {term}`cloud` properties.  In essence, the rate of change of the {term}`cloud radiative effect` per Kelvin surface warming.

  The current best estimate of the global-mean cloud feedback is that it is a mildly {term}`positive feedback`.

  However, these are highly uncertain, due to the large number of processes involved and the vast range of underlying physical scales, from micron-scale changes in e.g. cloud droplet size that influence cloud {term}`albedo` all the way up to changes in planetary-scale flow patterns that influence the overall location, extent, and height of different cloud types.  As such, a considerably more positive feedback, or even a slightly {term}`negative feedback`, cannot currently be ruled out.

  Of all the individual feedbacks, the cloud feedback contributes the greatest amount of uncertainty to the net feedback.

cloud radiative effect
  Essentially, the amount that the existence of {term}`cloud` alters the {term}`top of atmosphere` radiative balance.  Physical dimensions are power per unit area, so SI units are Watts per square meter ($\text{W m}^{-2}$).  Often abbreviated CRE.  
  
  Signed positive downward, i.e. into the atmosphere: positive CRE means that clouds cause a net *increase* of radiation to be absorbed within the climate system, whereas negative CRE means that clouds cause a net *decrease* of absorbed radiation.

  Can be defined for just the {term}`shortwave radiation` ("SW CRE"), just the {term}`longwave radiation` ("LW CRE"), or their combination ("net CRE"), which is just the sum of the SW CRE and LW CRE.  Each flavor can be defined/computed for the global average as well as locally.

  Globally averaged for Earth's present climate, the SW CRE is strongly negative, roughly $-50\text{ W m}^{-2}$, the LW CRE is moderately positive, roughly $+30\text{ W m}^{-2}$, and thus the net CRE is negative, roughly $-20\text{ W m}^{-2}$.  Thus, all together clouds act to cool Earth's climate.

  To be distinguished from {term}`cloud feedback`: whereas CRE refers to conditions for a given climate state, units $\text{W m}^{-2}$, cloud feedback is about the *change* in CRE with surface temperature change, units $\text{W m}^{-2}\text{ K}^{-1}$, as the system works toward a new equilibrium in response to some {term}`radiative forcing`.

  (More technically, CRE is computed using the numerical models of radiative transfer within {term}`climate model`s.  For a given state of the atmosphere, the radiative transfer code is run once to get the "all-sky" conditions.  The code is then repeated but with all clouds artificially *removed* from the atmosphere to get the "clear-sky" conditions.  The CRE is then taken as the all-sky minus the clear-sky.  There are also methods to try to compute it from observational data without relying on a numerical model, which we won't go into.)
  
  (We don't cover it, but one can also define a *surface* CRE: how much the radiative imbalance at the *surface*, rather than at TOA, is affected by clouds.)

control simulation
  A simulation in a given {term}`climate model` with all boundary conditions including greenhouse gas concentrations held constant the whole time.

  A.k.a. "control run"
  
  Any variability the model simulates is necessarily due to natural, {term}`internal variability`
  
  (Whereas in, for example, an SSP-forced simulation or doubled CO2 simulation, the model behavior has contributions from both natural variability and the imposed {term}`radiative forcing`.)

Coriolis parameter
  Conceptually, this tells us the strength of Earth's rotation on horizontal motions in the atmosphere.  
    
  Formally, we denote it $f$, and it is defined as $f=2\Omega\sin\varphi$, where $\Omega=2\pi\text{ radians} / (86400\text{ s})$ is the planetary rotation rate in SI units ($(1\text{ day})\times(24\text{ hr day}^{-1})\times(3600\text{ s hr}^{-1})$) and $\varphi$ is latitude (in radians).

  Why does it depend on the sine of latitude, $\sin\varphi$?  
  - At the poles where $\sin\varphi=1$ the horizontal plane is exactly **normal** to the rotation axis, meaning the Earth's spinning is exactly aligned with the local horizontal plane.  
  - At the equator, the horizontal plane is **parallel** to the rotation axis, meaning that the Earth's spinning is not occurring *at all* in the horizontal plane.  So at least for horizontal motions, at the equator it's as if the planet isn't rotating at all.
  - At latitudes in between, the horizontal plane is neither normal nor parallel to the rotation axis, and quantitatively the dependence is $\sin\varphi$.

cumulonimbus
  The deep clouds that extend from the surface sometimes all the way up to the {term}`tropopause, where they spread out laterally.  This gives them the overall shape reminiscent of a blacksmith's anvil, and hence the upper horizontally expansive part is called a cloud *anvil*.

  Caused by deep convection: very warm and moist air relative to the air above it becomes buoyant, which causes it to rise, creating cloud and heavy rainfall in the process.

  Taken as a whole, including both the narrower convective tower and the more expansive upper anvil, their net {term}`cloud radiative effect` is slightly positive: the trapping of {term}`longwave radiation` by both the tower and anvil win out over the reflection of {term}`shortwave radiation`.

  A useful starting point for thinking about the development of cumulonimbus clouds is to assume the air is undergoing {term}`adiabatic` ascent, and as such that its {term}`moist static energy` as it ascends through the troposphere is the same as the value it started with near the surface.

disequilibrium
  The opposite of {term}`equilibrium`.  For our purposes, this means that the climate system is *not* satisfying {term}`planetary energy balance`: either more is being absorbed than emitted at TOA, or vice versa.

  As such, when considering the planet as a whole and averaging long enough in time (i.e. over many decades), the global-mean surface temperature and other statistical measures of the climate are **not** *stationary*, meaning they *are changing*.

    Right now, due to historical {term}`anthropogenic` emissions of {term}`greenhouse gas` molecules and other activities, the climate system is in disequilibrium: the surface, {term}`troposphere`, and ocean are all warming up.

dry adiabatic lapse rate
  The {term}`lapse rate` followed by unsaturated air parcels that are rising or sinking {term}`adiabatic`ally.
  
  This can be derived exactly and is a global constant: \(\Gamma_\mathrm{d}\equiv g/c_p=9.8\text{ K km}^{-1}\), where $g$ is Earth's gravitational constant and $c_p$ is the specific heat of dry air at constant pressure.

emission
  For our purposes, this has two distinct meanings, both important:

  1. The release of molecules from the surface or by human activities into the atmosphere.  Of our primary concern is the emission of {term}`greenhouse gas` molecules such as CO2.
  2. The process of a substance sending out photons into its surroundings.

emission height
  The height above the surface at which the atmospheric temperature is equal to the blackbody temperature corresponding to Earth's outgoing longwave radiation (OLR).  Physical dimensions are height, so SI units are meters, but it's usually expressed in kilometers.

  Considering the global mean, for Earth's present climate the emission height is roughly 5-6 km above the surface.

emission temperature
  Given the planet's global-mean {term}`outgoing longwave radiation` (OLR) in Watts per square meter, the corresponding blackbody temperature.  Usually denoted $T_E$.  Physical dimensions temperature; SI units Kelvin.

  Symbolically, using the {term}`Stefan-Boltzmann law` for the blackbody radiation, we have $T_E=(\text{OLR}/\sigma)^{1/4}$.

emissivity
  Given the amount of radiation emitted by a body $E$ and its actual temperature $T$, the fraction that radiation is compared to if the body was a perfect blackbody.  Dimensionless and therefore unitless.  Denoted with a lower-case Greek epsilon, $\epsilon$.

  Putting the above description symbolically: $\epsilon=E/(\sigma T^4)$, since by the {term}`Stefan-Boltzmann law` the blackbody radiation is $\sigma T^4$.

  It is a *spectral* property, meaning it depends on the wavelength of the radiation being considered: $\epsilon=\epsilon(\lambda)$.  At any wavelength, it is identical to the {term}`absorptivity` (by [Kirchhoff's law of thermal radiation](https://en.wikipedia.org/wiki/Kirchhoff%27s_law_of_thermal_radiation)): if a body emits 70\% of the radiation at a given wavelength that a blackbody would at the same temperature, it also *absorbs* 70% of the radiation at that wavelength that it receives.

  For Earth's atmosphere, there are multiple {term}`absorption band`s within the {term}`longwave radiation` portion of the spectrum where both the emissivity and absorptivity are high.

equilibrium
  For our purposes, this means that the climate system is satisfying {term}`planetary energy balance`.

  As such, when considering the planet as a whole and averaging long enough in time (i.e. over many decades), the global-mean surface temperature and other statistical measures of the climate are *stationary*, meaning they do not change.

  If a system is not in {term}`equilibrium`, then it is in {term}`disequilibrium`.

  Right now, due to historical {term}`anthropogenic` emissions of {term}`greenhouse gas` molecules and other activities, the climate system is *not* in equilibrium.

  (Strictly speaking, Earth's climate is never *truly* in equilibrium, because its orbit is constantly, albeit slowly changing, and the carbon cycle is slowly changing the greenhouse gas concentrations, etc.  But those are slow enough processes---tens of thousands or hundreds of thousands of years or more---compared to the timescale of physical equilibration of the atmosphere and ocean, more like a few thousand years---that it is still useful to *approximate* the climate as being in equilibrium or not.)

equilibrium climate sensitivity
  The {term}`climate sensitivity` after the whole climate system, including the deep ocean, reaches a new {term}`equilibrium` state.  

  This takes *thousands* of years, because of two factors.  Considering a *positive* {term}`radiative forcing` to be definite (but just reverse all the signs for the case of a *negative* one), these are:
  
  1. The vast majority of excess energy being received by the climate system due to the positive radiative forcing is absorbed by the ocean, nearly all of it in a thin layer near the surface.  For ongoing {term}`anthropogenic` climate change, this is around 90\%.
  2. The deep ocean has a huge heat capacity, and the mixing of energy throughout its expanse is extremely slow, in part because the circulation of water itself is very slow in the deep ocean.

  Combined, these result in it taking a very long time, millennia, for all of the heat absorbed initially in the upper ocean layer to warm up the rest of the deep ocean, and thus for the system to fully reach a new equilibrium.

extratropics
  Everything poleward of the {term}`tropics`, in both the Northern Hemisphere and Southern Hemisphere.

  There is no hard boundary betwen the tropics and extratropics, but commonly for Earth we use $30^\circ$S and $30^\circ$N to demarcate the two zones.  Using that, the extratropics is $30^\circ-90^\circ$S in the Southern Hemisphere and $30^\circ-90^\circ$N in the Northern Hemisphere.

  In the extratropics, the {term}`Coriolis parameter` is large enough that Earth's rotation very strongly influences large-scale horizontal motions.  This, combined with the meridional temperature gradient between the warm low latitudes vs. much colder poles, gives rise to the large-scale cyclonic storms called baroclinic eddies. 

eye
  For our purposes, the calm, clear, central part of a {term}`tropical cyclone`.

eyewall
  The part of a {term}`tropical cyclone` directly outside of the {term}`eye`.  The eyewall is home to the strongest ascent and most severe rainfall.  
  
  It is totally filled by thick clouds which surround the clear eye, forming, metaphorically speaking, a "wall" around the eye.  Hence the term *eyewall*.

floe
  A piece of floating ice.  For our purposes, this is {term}`sea ice` and can be any size, from a few cm wide at its widest point to hundreds of kilometers.

glacier
  A large piece of ice sitting on a mountain.

  Melt of glaciers with warming contributes to {term}`sea level rise`, since the water molecules that were locked in the glacier as ice melts and flows downslope as liquid water, ultimately reaching the oceans.  (At least, some fraction of the melted water does; some of it may end up in ground storage.)

  Conversely, in the case of *cooling* rather than warming, the accumulation of water molecules as ice locked in the glacier contributes to sea level *decrease*.

greenhouse gas
  A molecule in Earth's atmosphere that significantly absorbs {term}`longwave radiation`.  The two most important ones are carbon dioxide (CO$_2$) and water vapor (H$_2$O).  Others include methane (CH$_4$), nitrous oxide (N$_2$O), and ozone (O$_3$)

greenhouse effect
  The warming of Earth's surface due to the absorption by {term}`greenhouse gas`es in Earth's atmosphere of Earth's emitted {term}`longwave radiation` and subsequent reemission of longwave radiation back downward to the surface

  Human emissions of greenhouse gases are acting to increase the strength of the greenhouse effect, thereby warming Earth's surface.  But note that the greenhouse effect exists even absent human activities; we humans are *changing* it, but we didn't *create* it.
  
  Without the greenhouse effect, the surface temperature would be the same as the {term}`emission temperature`.

  (Beware: the term "greenhouse effect" is kind of a misnomer...it's similar but different to the way an actual greenhouse for plants stays warm inside.)

Hadley cells
  The time-mean, zonal-mean overturning circulation in Earth's {term}`tropics`.  
  
  Upward motion in their ascending branch in the deep tropics fuels the heavy rainfall of the {term}`Intertropical Convergence Zone` near the equator.  Sinking in their descending branches promote aridity in the subtropics of both the Northern Hemisphere and Southern Hemisphere.

hiatus periods
  During the transient period of warming in response to a positive {term}`radiative forcing`---such as the ongoing global-mean warming in response to historical {term}`anthropogenic` greenhouse gas emissions---periods of roughly a decade or longer during which global-mean surface temperature nonetheless stays flat or even slightly cools.

  These are the natural consequence of two things happening at once: (1) the long-term warming due to the system trying to reach a new equilibrium, and (2) natural, {term}`internal variability` in the climate system that causes the surface to be a bit warmer than usual or--in the case of hiatus periods---a bit colder than usual for a while.

high cloud
  A {term}`cloud` that is sufficiently high in Earth's {term}`troposphere`, say 7 km and higher.  Because temperatures there are very cold, often consist of ice crystals or are *mixed-phase*, meaning a combination of liquid droplets and ice crystals.
  
  For our purposes, notable types of high floud include wispy *cirrus* clouds and the thick *anvil* of {term}`cumulonimbus` towers. 

  High clouds tend to have a positive net {term}`cloud radiative effect`:
  - {term}`longwave radiation`: being high up to the surface, their temperature is typically much cooler than that of the surface, resulting in substantial net absorption of LW.  In other words, they absorb the LW emitted by the surface underneath, and then re-emit it at a much colder temperature and thus with less energy, resulting in less radiative energy escaping to space.
  - {term}`shortwave radiation`: they reflect SW back to space, so SW CRE is negative.
  - net: Generally positive: the LW trapping tends to win out over the SW reflection

hurricane
  Another name for a {term}`tropical cyclone`, specifically for those storms that form in the Atlantic Ocean and the Eastern Pacific.  These are the storms that affect Central America, the Caribbean, and North America.

ice sheet
  A huge mass of ice on land.  Currently, there are two: Greenland and Antarctica.  
  
  In colder periods such as the ice ages, these were thicker and more expansive, and the great Laurentide ice sheet extended beyond Greenland to much of the northern high latitudes, including much of Canada and northern Europe, and in North America reaching as far south as New Jersey, Pennsylvania, and Ohio.  The retreat of the ice sheets from glacial to interglacial periods affects local {term}`sea level rise` through {term}`post-glacial rebound`.

insolation
  A contraction of the phrase "**in**coming **sol**ar radi**ation**": the amount of solar radiation incident at Earth's {term}`top of atmosphere`.  Physical dimensions are power per area; SI units are Watts divided by square meter, $\text{W m}^{-2}$.

Intertropical Convergence Zone
  The time-mean, zonal-mean band of high precipitation in Earth's deep tropics.
  
  Often referred to by its acronym, the ITCZ.

  Driven in large part by the upward motion within the ascending branch of the {term}`Hadley cells`.

internal variability
  A.k.a. "natural variability."  The naturally occuring ~random-ish fluctuations that occur on many different timescales in Earth's atmosphere and ocean.  Even for global-mean surface temperature, such internal variability can result in several years or even multiple decades of warming or cooling.

  That is even more the case when considering smaller scales.  In general, the smaller the timescale and/or spatial scale, the greater influence internal variability will have on the behavior relative to other factors.

inverse square law
  For our purposes, the fact that the amount of solar radiation *per unit area* decreases with the square of the distance away from the sun.

  Formally, if $L$ is the sun's luminosity in Watts, $r$ is radial distance from the sun in meters, and $E$ is the radiative intensity per unit area, units Watts per square meter, then $$E=\frac{L}{4\pi r^2}$$

  Intuitively, very close to the sun, all of the emitted photons are traveling outward through a very small sphere in space.  As they travel outward, the number of photons doesn't change, but the area of the sphere grows and grows as $4\pi r^2$.  So the amount of photons *per unit area* decreases.

  This is what makes a planet's distance from the sun so fundamental to its climate.

  Even still, it's not the only factor: the 

  For more: [Wikipedia page](https://en.wikipedia.org/wiki/Inverse-square_law)

low cloud
  A {term}`cloud` that is sufficiently low in Earth's {term}`troposphere`, so anywhere from the surface up to say 3-4 km.  Of our particular interest are the pervasive decks of *stratocumulus* clouds over the eastern portions of the subtropical oceans.

  Low clouds tend to have a negative net {term}`cloud radiative effect`:
  - {term}`longwave radiation`: being close to the surface, their temperature is not usually much cooler than that of the surface, resulting in little net absorption of LW.  So, even though they are highly effective absorbers of surface LW, they then re-emit it at nearly the same temperature: LW CRE is close to zero
  - {term}`shortwave radiation`: they reflect lots of SW back to space, so SW CRE is strongly negative.
  - net: Little LW absorption plus strong SW reflection equals negative CRE.

Kelvin
  Absolute temperature, such that zero Kelvin equals [absolute zero](https://en.wikipedia.org/wiki/Absolute_zero).  Abbreviated K.  The SI unit for temperature.  Equal to degrees Celsius plus 273.15.  

  Because it has the identical *spacing* as degrees Celsius, for quantities that represent *differences* in temperature the two units can be used interchangeably.  For example, when we say the planet warms up by a given amount, that refers to the new temperature *minus* the old temperature, and so it is the same number in Kelvin as degrees Celsius.

  Conversely, if we were talking about Earth's current global-mean temperature, which is approximately 288 Kelvin, that is **not** the same as $288^\circ\text{C}$.  It *is* the same as $288-273.15=14.85^\circ\text{C}$.
  
  Another example, we can say that the average {term}`lapse rate` in the troposphere is approximately 6 Kelvin per kilometer, or just as well that it is 6 degrees Celsius per kilometer.  That's because the lapse rate is the *change* in temperature with height, i.e. the (infinitesimal) difference in temperature between two adjacent heights.

land ice
  Ice that sits on land.  This includes the Greenland {term}`ice sheet`, Antarctic {term}`ice sheet`, and all mountain {term}`glacier`s.

lapse rate
  The change in temperature with height, with sign flipped.  Usually denoted with a capital Gamma $\Gamma$: $\Gamma\equiv-\partial T/\partial z$.  Physical dimensions are temperature divided by height, so SI units are Kelvin divided by meters, but the denominator is often expressed in kilometers, so $\text{K km}^{-1}$, or equivalently $^\circ\text{C km}^{-1}$.

lapse rate feedback
  The {term}`radiative feedback` due to changes in the {term}`lapse rate` as the climate responds to a {term}`radiative forcing`.

  Globally, the lapse rate feedback is a {term}`negative feedback`.

  Regionally, it is most negative in the Tropics due to the amplified warming aloft associated with the approximately moist adiabatic lapse rate there.  At higher latitudes, due to an inversion in temperature near the surface, the lapse rate feedback is a {term}`positive feedback`.

longwave radiation
  Essentially, the radiation emitted by the Earth.  This corresponds to electromagnetic radiation with wavelengths spanning approximately 5-80 {term}`micron`.  Commonly abbreviated to LW.  Units are Watts divided by square meter, $\text{W m}^{-2}$.

  To be contrasted with {term}`shortwave radiation`, which essentially is the radiation emitted by the sun.

micron
  Another name for a micrometer.  The micro prefix means one-millionth and is denoted with a greek mu: $\mu$.  So one micron equals one millionth of a meter, or one thousandth of a millimeter: $1\;\mu\text{ m}=10^{-6}\text{ m}=10^{-3}\text{ mm}$

model uncertainty
  From *Hawkins and Sutton 2007*, the uncertainty in future projections of some climate variable stemming from differences across climate models.

  For a given field of interest---meaning the physical quantity, time period, and spatial region---and a given future scenario of interest, suppose that all of the available state-of-the-art climate models perform the identical simulation.  Because of differences in how the models are formulated, there will be differences across the models in the change in the particular field.

  Be aware:  in this example, if only a single run is performed with each model, there will also be a contribution to the across-model differences from {term}`internal variability`: each model's simulation will have its own unique realization of its internal weather and other natural fluctuations, in addition to the differences across models due to their different formulations.  
  
  As such, a better experimental design to isolate model uncertainty is for each model to perform a large *ensemble* of runs, each identically forced but starting from slightly different initial conditions.  Then, averaging across each model's ensemble would act to remove the internal variability component, and then one would compare these individual model ensemble averages across the models.

moist static energy
  A commonly used representation of the energy per unit mass of a moist air parcel in Earth's atmosphere.  Often abbreviated MSE.  It is the sum of three terms: $\text{MSE}=c_pT+gz+L_vq$: 
  - $c_p$ is the specific heat of air at constant pressure, $T$ is temperature in Kelvin, and their product represents the parcel's *thermal energy*
  - $g=9.81\text{ m s}^{-2}$ is Earth's gravitational constant, $z$ is height in meters, and their product represents the parcel's *potential energy*
  - $L_v=2.5\times10^{6}\text{ J kg}^{-1}$ is the latent heat of vaporization of water, $q$ is {term}`specific humidity` (dimensionless), and their product represents the heat that would be released if all of the parcel's water vapor condensed into liquid water

negative feedback
  For our purposes, a {term}`radiative feedback` that acts to *damp* an existing radiative *imbalance* at the {term}`top of atmosphere`.  A.k.a. *stabilizing* feedback or *inhibiting* feedback.  As such, negative feedbacks act to weaken suface warming.

  For the global mean, the key negative feedbacks are the {term}`Planck feedback` and {term}`lapse rate feedback`.
  
  The global-mean net radiative feedback is negative: in response to a positive {term}`radiative forcing`, as the surface air temperature increases, the TOA radiative imbalance decreases, and so the system evolves toward a new equilibrium.  
  
  (If, instead, the global-mean net radiative feedback was *positive*, it would be impossible to regain TOA balance!  As the system warms, the excess energy into the system at TOA would *increase*, further amplifying the initial warming.  This is known as a *runaway greenhouse* and is thought to have occured on Venus.)

one-layer greenhouse model
  The simplest {term}`analytical framework` for understanding a planet's {term}`greenhouse effect`.

  All of the processes affecting both {term}`longwave radiation` and {term}`shortwave radiation` within the atmosphere are boiled down to a single layer of atmosphere.  Any {term}`absorption` of {term}`shortwave radiation` within the atmosphere is neglected---meaning all of the SW absorption occurs at the surface.  Whereas for {term}`longwave radiation`, the atmosphere absorbs some of the LW emitted by the {term}`surface`, with the fraction absorbed determined by the atmosphere's {term}LW `emissivity`, $\epsilon$.
  
  For {term}`emission`, the atmospheric layer has a temperature $T_a$ and emits LW according to the {term}`Stefan-Boltzmann law`: $\sigma T_a^4$, multiplied by its {term}`emissivity` $\epsilon$ to account for the fact that it is an *imperfect* {term}`blackbody`.

  This single-layer atmosphere emits LW $\epsilon\sigma T_a^4$ both upward and downward.  The upward flux escapes to space and therefore determines the planet's {term}`outgoing longwave radiation`.  The downward flux is absorbed by the {term}`surface`.

  It is the partial absorption of the surface's emitted LW radiation by the atmosphere, the subsequent re-emission of this absorbed LW back downward by the atmosphere, and the surface's absorption of that extra downwelling LW from the surface, that ultimately warms the surface.

outgoing longwave radiation
  The upward flux of longwave radiation at the top of the atmosphere, in units Watts divided by square meter, $\text{W m}^{-2}$.  Commonly abbreviated to OLR.  *Outgoing* means that it is signed positive out of the atmosphere.  The global-mean value at present is roughly $240\text{W m}^{-2}$.

photon
  A single indivisble particle of electromagnetic radiation.

  Because of the {term}`wave-particle duality` that is inherent to all EM radiation, one can think of EM radiation as either a discrete photon or as a continuous wave, flipping back and forth between the two perspectives as is convenient.

  A photon's energy is given by $E=h\nu$, where $h=6.626\times10^{-34}\text{ J s}$ is **Planck's constant**, and $\nu$ is the **frequency**.  Thus, the *faster* the frequency, the *more* energy the photon carries.

Planck feedback
  The {term}`radiative feedback` stemming directly from the {term}`Stefan-Boltzmann law`: blackbody emission increases with temperature to the fourth power, and so all else equal if the surface temperature and rest of the troposphere warm up by some amount, the {term}`outgoing longwave radiation` will increase, acting to reduce the net imbalance at the {term}`top of atmosphere` that led to the initial warming.

  Globally averaged, it is the single largest {term}`negative feedback`.

  Regionally, it contributes to {term}`polar amplification` because the increase in radiation per unit warming itself increases with the original temperature.  As such, warming in the Tropics---where it's already warm---leads to a larger increase in emitted {term}`longwave radiation` compared to the same warming near the poles where, compared to the Tropics, it's much colder.

planetary albedo
  The {term}`albedo` averaged in time and over the whole planet, and considering the fluxes of {term}`shortwave radiation` at the {term}`top of atmosphere`.

   Planetary albedo is often denoted $\alpha_p$ and for Earth's present climate is approximately 0.3: approximately 30% of the insolation is reflected back to space, meaning that remaining 0.7 or 70% is absorbed within the climate system.

  (The term "{term}`albedo`" without the "planetary" part is more general: it can refer to a particular location and time rather than averaging over the whole planet.)

planetary energy balance
  Intuitively / informally: at {term}`equilibrium`, energy absorbed by the climate system must be balanced by energy lost by the climate system.

  For Earth's climate, the vast majority of energy *received* is in the form of {term}`shortwave radiation` emitted by the sun.  (Energy received through all other sources, for example geothermal heating, is tiny by comparison in the global average.)    Similarly, virtually all of the energy *lost* by the climate is in the form of {term}`outgoing longwave radiation`, OLR: photons emitted by the planet itself, in the form of {term}`longwave radiation` that escape to space.  
  
  Together, these imply that the location where we measure the planetary energy balance is the {term}`top of atmosphere` (TOA).

  To go from the {term}`insolation` to the amount of {term}`shortwave radiation` *absorbed*, we take into account the {term}`planetary albedo`, i.e. the fraction of the {term}`insolation` at the {term}{top of atmosphere} that is reflected back to space rather than absorbed.  If $S_0$ is the {term}`solar constant` and $\alpha_p$ is the {term}`planetary albedo`, then $S_0(1-\alpha_p)$ is the global-mean TOA SW absorbed, in $\text{W m}^{-2}$.

  As such, the planetary energy balance depends on the balance between the *net* downwelling SW and the OLR at TOA.
  
  If planetary energy balance is satisfied, then the climate system is in {term}`equilibrium`.

  In the presence of a planetary energy *imbalance*, the system is in {term}`disequilibrium` and will respond in some way that ultimately restores balance at the TOA.  
  
  If the *sign* of that imbalance is that there is more SW being absorbed than OLR, then the system will tend to *warm up* in order to increase the amount of OLR.

polar amplification
  The tendency for surface temperature increases in response to positive {term}`radiative forcing` such as increased CO$_2$ to be greater near the poles than at lower latitudes.  This is especially true for the Arctic, and so sometimes it's referred to as *Arctic amplification*.  
  
  There are three key {term}`radiative feedback` processes that contribute to polar amplification, in each case due to that feedback being more stabilizing at lower latitudes than at higher latitudes: (1) {term}`Planck feedback`, (2) {term}`surface albedo feedback`, and (3) {term}`lapse rate feedback`

  For the Antarctic, the prevailing upwelling of cold water from depth in the Southern Ocean tends to delay the warming in the southern high latitudes.

positive feedback
  For our purposes, a {term}`radiative feedback` that acts to *amplify* an existing radiative *imbalance* at the {term}`top of atmosphere`.  A.k.a. an *amplifying* feedback.  As such, positive feedbacks act to amplify suface warming.

  For the global mean, the key positive feedbacks are the {term}`water vapor feedback` and {term}`surface albedo feedback`.  The {term}`cloud feedback` is most likely positive too, but it is subject to much more uncertainty.

  Note: in response to a *negative* {term}`radiative forcing`, the overall surface air temperature response will be negative, i.e. cooling.  In that case, a "positive" feedback *amplifies* the temperature change, i.e. contributes *more* cooling, not less.  (That's why the "positive" vs. "negative" terms are a little confusing compared to "amplifying" vs. "inhibiting".)

post-glacial rebound
  During the Ice Ages---the most recent one being the Last Glacial Maximum that peaked roughly 21,000 years ago---huge ice sheets several kilometers thick develop over the continents.  The weight of this huge mass of ice pushes the local land surface down.  After they retreat in the subsequent *interglacial* period such as we're in right now, the land that was underneath them gradually rises up.  This acts to reduce local sea level.

  The growth and retreat of the ice sheets also indirectly causes the nearby land surface to move up and down even past where the ice sheet ever reached: when the ice sheet pushes the land beneath it down, some of the crust also gets pushed out to the side in addition to downward.  This adds land mass to adjacent areas and thus causes the land surface there to go up, decreasing the local sea level.  Going from the glacial to the interglacial, the reverse process occurs: where the ice retreats, the land moves up but also some crust flows toward it, which acts to decrease the surface height in adjacent areas and thus cause local sea level rise.

radiative feedback
  A process driven by the change in Earth's *surface* temperature that results in a change in the net {term}`top of atmosphere` radiative flux.  More formally, the change in Watts per meter squared at TOA per Kelvin change in surface temperature.
  
  Any particular radiative feedback can be a {term}`positive feedback` or a {term}`negative feedback`.
  
  The key individual feedbacks for Earth's present-day climate are the {term}`Planck feedback`, {term}`water vapor feedback`, {term}`lapse rate feedback`, {term}`surface albedo feedback`, and {term}`cloud feedback`.

  The **net** radiative feedback is the sum of all these individual feedback processes.  The net global-mean feedback must be negative; otherwise the TOA radiative imbalance would only grow and grow, and a new equilibrium would never be reached.

  In addition to global-mean feedbacks, the feedbacks can be analyzed regionally, for example to help understand the causes of {term}`polar amplification`.

radiative forcing
  The net radiative imbalance at the {term}`top of atmosphere` immediately following some perturbation imposed externally on the climate system.

  Think of it as quantifying how "hard" the system has been hit: the larger the radiative forcing, the more the climate will have to change in order to reach a new equilibrium that balances that radiative forcing.
  
  Physical dimensions are power per unit area, and so SI units are Watts per square meter.  Signed positive *downward*: positive if there's a net *surplus* of radiation entering the climate system, i.e. more radiation absorbed than emitted.  Negative if, instead, there's a net *deficit*: more being emitted to space than being absorbed.

  The example of our particular interest is the radiative forcing due to an instantaneous doubling of atmospheric $\text{CO}_2$, which is approximately $4\text{ W m}^{-2}$.  But the concept of radiative forcing can be applied to any other imposed perturbation to the climate system too, e.g. historical {term}`anthropogenic` aerosol emissions, or changes in {term}`insolation` due to solar cycles or orbital variations.

  It's not something that can be directly measured, so we infer it from climate model simulations.

  (Strictly speaking, there is a meaningful distinction between the TOA imbalance that arises *instantaneously* after the perturbation is applied and the TOA imbalance after say a few weeks, a time period that's long enough that the atmosphere adjusts to some extent but short enough that the more sluggish surface temperature hasn't changed much yet.  The TOA imbalance after this "rapid adjustment" is referred to as *effective radiative forcing* (ERF), and long-term warming is better predicted by the ERF than the *instantaneous* radiative forcing.  But we won't worry about that distinction in this course.)

relative humidity
  For our purposes, the {term}`specific humidity` divided by the {term}`saturation specific humidity`.  It is a dimensionless quantity.  It can range from zero if the air is completely dry up to 1, i.e. 100%, if the air is saturated.  Often abbreviated RH.

  Under climate change, it happens to be the case that the relative humidity within the troposphere doesn't change by a lot.  Combined with the rapid increase of {term}`saturation specific humidity` with warming due to the {term}`Clausius-Clapeyron` equation, this results in strong increases in the amount of water vapor in the atmosphere with warming.

  Relative humidity can also be above 100% in cases of *supersaturation*, which can occur if there aren't enough {term}`aerosol` particles in the air that can act as cloud condensation nuclei that the water can condense onto, forming cloud droplets.

  (More precisely, relative humidity is defined as the partial pressure of water vapor divided by the saturation partial pressure of water vapor.  But this ratio in terms of partial pressures is very closely approximated by the ratio in terms of specific humidities, and specific humidity is the more directly relevant quantity for things we care about such as radiative transfer and {term}`moist static energy`.)

saturation
  The condition of an air parcel where, given its temperature and {term}`specific humidity`, the parcel holds exactly as much water vapor as it can without any of the water vapor condensing into liquid.  This is determined by {term}`Clausius-Clapeyron`.

  In terms of {term}`relative humidity` (RH), saturation is identical to $\text{RH}=100\%$.

  You can think of it as the air parcel being "at capacity" with respect to water vapor: any colder, or any more water molecules, the water vapor would start condensing.

saturation specific humidity
  Given an air parcel with a temperature $T$, the {term}`specific humidity` value that air parcel would have if the parcel was at {term}`saturation`.

scattering
  In radiative transfer, when a photon hits a molecule and is "bounced" to a different direction.  Unlike in {term}`absorption`, the photon continues to exist and has the same wavelength and hence energy as it did before encountering the molecule.
  
  This doesn't have to be reflection straight back in the original direction; it can be a more modest change in angle.  But for our purposes what's really important here is when a {term}`shortwave radiation` photon traveling downward toward Earth's surface gets reflected back up, either by the surface or within the atmosphere.

  (The photon's *polarization*, meaning the direction of its wavefronts, can be changed as well, but we won't be concerned with the polarity of EM radiation in this course.)

scenario uncertainty
  From *Hawkins and Sutton 2007*, the uncertainty in future projections of some climate variable stemming from uncertainty in what will happen societally regarding greenhouse gas emissions and other anthropogenic influences on climate.  
  
  It's possible that, for example, a political breakthrough and/or technological breakthrough cause emissions to go down rapidly.  It's also possible that, for example, political deadlock on carbon policy or unexpectedly rapid population growth cause emission to continue increasing for the rest of the century.  Or anything in between.

  Unlike {term}`internal variability` and {term}`model uncertainty`, this is not a source of uncertainty that can be directly addressed via the physical climate science and climate models we are otherwise mostly learning about in this class.  Instead, it's more in the realm of economists, political scientists, etc. who try to model the actions of individuals, firms, nations, etc.

sea ice
  Ice that is floating in the oceans or seas.  Has a high {term}`albedo`.

  An important contributor to {term}`surface albedo feedback`: in response to warming, sea ice will melt, exposing much darker ocean underneath, leading to more absorption of {term}`shortwave radiation`.

  Conversely, sea ice melting (or expansion in the case of cooling) does not meaningfully contribute to {term}`sea level rise`, because---unlike land ice---it is already floating: by Archimedes' Principle floating sea ice displaces its weight in liquid water, so when it melts there is no change in the ocean's volume.

sea ice area
  Looking down from space, the total area covered by {term}`sea ice`.  Often considered for the Arctic as a whole and, separately, for the Antarctic as a whole.  Physical dimensions are area, so units meters squared, but often expressed in millions of square kilometers: $10^6\text{ km}^2$.

sea ice age
  How long a given piece of {term}`sea ice` has existed, starting from when it first formed.  Dimensions are time.

sea ice concentration
  The fraction of a specified grid box's area that is covered by {term}`sea ice`.  Dimensionless, and thus unitless; typically expressed in percent.

  (Can depend to some extent on the precise grid box boundaries.)

sea ice extent
  The area spanned by grid boxes with {term}`sea ice concentration` exceeding a specified threshold, usually taken to be 15%.   Physical dimensions are area, so units meters squared, but often expressed in millions of square kilometers: $10^6\text{ km}^2$.

  (As for sea ice concentration itself, can depend to some extent on the precise grid box boundaries.)

sea ice thickness
  The vertical extent of a given piece of {term}`sea ice`, from its bottom below the ocean surface to its top just above the ocean surface.  Physical dimensions are distance, so SI units meters.

sea level rise
  The increase in the height of the ocean surface that occurs with surface warming.  Often abbreviated SLR.  Caused by changes in the total volume of the ocean.

    Globally averaged, there are three key contributors: 
    - {term}`steric sea level rise`
    - melting of land ice, i.e. ice sheets and mountain glaciers
    - changes in land water storage

    At any particular coastal location and timescale, the rate and sign of SLR depends on several additional factors as well:
    - *atmospheric pressure loading*: higher pressure = atmosphere heavier = pushing down on ocean surface more = sea level goes down
    - *wind stress*: wind blowing over ocean surface = pushes water with it = water piles up in the direction the wind is blowing toward, goes down in the direction the wind is blowing away from (at sufficiently large length scales, this is strongly altered by Earth's Coriolis effect, with instead the net transport of water being at a right angle to the surface wind direction)
    - *tides*: The roughly twice-daily cycle of tides caused by the moon's gravitation causes sea level to rise and fall at the coastline, in some places by several meters.
    - *storm surge*: Strong winds directed onshore during a tropical cyclone or other strong storm push ocean water onto the land, temporarily increasing local sea level
    - *coastal erosion*: over time, beaches get eroded by storms, causing the local land height at the coast to decrease and thus the local sea level to increase
    - {term}`post-glacial rebound`
    - *gravitational effects of ice sheet melt*: ice sheets sit vertically above the ocean surface, and gravity pulls ocean water nearby upward toward the giant mass of ice.  This raises the local sea level, and the sea level farther away must go down to compensate.  Because of all this, when the ice melts, the local upward gravitational pull weakens, acting to decrease local sea level and increase sea level farther away---at least, relative to the global-mean sea level, since the ice sheet melt itself will act to increase sea level overall by adding water mass to the ocean.

shortwave radiation
  Essentially, the radiation emitted by the Sun.  This corresponds to electromagnetic radiation with wavelengths spanning approximately 0.1-2 {term}`micron`.  Commonly abbreviated to SW.  Units are Watts divided by square meter, $\text{W m}^{-2}$.

  To be contrasted with {term}`longwave radiation`, which essentially is the radiation emitted by the Earth.

solar constant
  The average amount of radiative energy from the sun arriving at a planet, per unit time and per unit area.  Physical dimensions are power per unit area, so SI units are Watts per square meter, $\text{W m}^{-2}$.  Denoted $S_0$.

  For modern Earth, this is $S_0\approx1340 \text{W m}^{-2}$.

  A planet's solar constant is determined by the {term}`inverse square law`, and depends on its average distance from the sun $d$ and the sun's luminosity $L_0$.

specific humidity
  For a given volume of air, the mass of water vapor divided by the total air mass.  Usually denoted $q$.  Dimensionless: kg / kg.

Stefan-Boltzmann law
  The equation for how much energy per unit area that a {term}`blackbody` emits, in units Watts per square meter: $E=\sigma T^4$, where $T$ is the blackbody's temperature and $\sigma=5.67^10^{-8}\text{ W m}^{-2}\text{ K}^{-1/4}$ is the Stefan-Boltzmann constant

steric sea level rise
  The component of sea level rise that stems directly from changes in the seawater *density*.  Water expands as it warms, and so warming of the ocean induces a steric sea level rise directly even if there was no extra mass of water added: the same amount of water takes up more space, and so it has to go up.

stratosphere
  The layer of Earth's atmosphere directly above the {term}`troposphere`, extending from the {term}`tropopause`

stratospheric cooling
  The fact that, in response to increased atmospheric $\text{CO}_2$, the {term}`stratosphere` tends to cool at the same time that the {term}`troposphere` warms.

subtropics
  The mostly arid, poleward portion of the {term}`tropics`.  There are no hard boundaries, but we often use $15-30^\circ$ latitude in either hemisphere to define the subtropics.

  The descending branches of the {term}`Hadley cells` are located in the subtropics, which is a large contributor to the presence of deserts and dry atmospheric conditions more generally in the subtropics.

surface
  For our purposes, the *surface* refers to the surface of the planet, meaning the boundary separating the {term}`atmosphere` above, which is (mostly) gas, from what's below: depending on the location, that's either liquid (oceans, lakes, etc.) or solid (land or ice).

  Among other reasons, we care about conditions at Earth's surface because, well, that's where we live.

surface albedo
  The {term}`albedo` at the planet's {term}`surface`.  So, given the amount of downwelling {term}`shortwave radiation` hitting the surface, the *fraction* of that SW that is reflected back up by the surface rather than absorbed.

  Being a fraction, it is dimensionless and therefore unitless.  Its minimum is 0, meaning every SW {term}`photon` that hits the surface gets absorbed and none get reflected back up.  Its maximum is 1, meaning every SW {term}`photon` that hits the surface gets reflected back up and none get absorbed.

  Broadly, the *darker* the surface, the *lower* the albedo, meaning *more* of the SW is absorbed.  So, for example, the dark blue oceans have a lower surface albedo than bright white {term}`sea ice`.
  
  This can be for a specific location/region and/or time.  You can also average it in space and time to give you a value of the planetary surface albedo.

  The *surface* albedo is distinct from---but influences---the {term}`albedo` at the {term}`top of atmosphere`.  The TOA albedo depends on the surface albedo: if a photon from the sun passes through the atmosphere but gets absorbed at the surface, then with respect to the TOA radiative flux, this will increase

  (The surface albedo and the albedo at TOA are not identical because {term}`absorption` and {term}`scattering` of SW photons occurs not just at the surface but also within the atmosphere.  For example, clouds are bright and thus increase the TOA albedo, but this doesn't directly affect the surface albedo.)

surface albedo feedback
  In response to a positive {term}`radiative forcing` (such as increased CO$_2$), a *decrease* in {term}`surface albedo` as the planet warms up, making it harder to restore {term}`planetary energy balance`.
  
  In more detail, surface temperatures increase, causing some ice and snow will melt, which exposes darker ocean or land surface underneath and thus causes more {term}`shortwave radiation` to be absorbed.  This acts to increase the original positive radiative forcing and thus amplify the warming, compared to the hypothetical case if the {term}`surface albedo` had remained unchanged.  It thus constitutes a {term}`positive feedback` in the global mean.

  It promotes {term}`polar amplification` because the ice and snow occurs at high latitudes, so the extra shortwave absorption is concentrated in high latitudes promoting more rapid local warming compared to lower latitudes, all else equal.

top of atmosphere
  The top of the atmosphere.  Commonly abbreviated as TOA.  Important because it constitutes the outer boundary of the whole climate system.  So, for planetary energy balance, the net energy flux across the TOA must be exactly zero for Earth's climate to be in equilibrium.
  
  (In reality, there is no true, well-defined "top" of the atmosphere, with the atmosphere below and outer space above.  Instead, the atmosphere gradually thins moving higher and higher up.  But for practical purposes, it is completely kosher and useful to act as if there is one.)

transient climate sensitivity
  In response to some imposed {term}`radiative forcing`, the response of surface temperature *before* the deep ocean---and thus the full climate system---has fully equilibrated.

  This could be, for example, in the first decade, or first century, or any other time period before the system has fully equilibrated.  It is always *smaller* than the {term}`equilibrium climate sensitivity`, because the system gradually asymptotes toward its equilibrium state over thousands of years, after an initial fairly rapid period of change in the first century or so.

  (There is a related, more precisely defined quantity in climate science called the *transient climate response*, or TCR, which is the global-mean surface air temperature change at the time that atmospheric $\text{CO}_2$ concentration reaches twice its original concentraiton in a climate model simulation where the atmospheric $\text{CO}_2$ concentration is increased by 1% per year, each year.)

transmission
  In radiative transfer, when a photon encounters a molecule but simply passes right through it unchanged, as if the molecule wasn't even there.  This is to be contrasted with {term}`absorption` and {term}`scattering`, which are the other two possible outcomes when a photon meets a molecule.

  (This is by far the most common outcome within Earth's atmosphere.  Generally $>95\%$ of the atmosphere by mass consists of N$_2$ and O$_2$ molecules, which are almost completely inert and as such do not interact with either {term}`shortwave radiation` or {term}`longwave radiation`.)

tropical cyclone
  An intense, rotating storm that forms in the `term`{tropics} over warm ocean waters and that features a calm central {term}`eye`, a surrounding {term}`eyewall` with the most intense rainfall and winds, and a broader region of spiraling clouds, high winds, and rainfall.
  
  For North America, these are more popularly known as {term}`hurricane`s.  For East Asia, they are more popularly known as {term}`typhoon`.

tropics
  The portion of Earth near the equator that, generally, is warm and moist, due to the high {term}`insolation` it receives compared to higher latitudes.

  Another important feature of the tropics is that the {term}`Coriolis parameter` is small there, 
  
  There are no catch-all, exact boundaries of the Tropics, but commonly used definitions.

  The rest of the Earth, i.e. the part that is not the Tropics, is the {term}`extratropics`.

  Sometimes we distinguish between the *deep tropics*, roughly 15$^\circ$S-15$^\circ$N, which is the wettest part, from the {term}`subtropics`, roughly 15-30$^\circ$S and 15-30$^\circ$N, which is drier.

tropopause
  The boundary between the {term}`troposphere` and {term}`stratosphere`.  Typically around 10-15 km, with the higher values generally in the tropics and lower values in the extratropics.

  (Although we often treat it as a single height or pressure, in reality there is some finite-depth transition region between the troposphere and stratosphere, and even the position and depth of that transition layer can vary depending on the precise definition used.  But it is still very useful for us in this course to treat it as being a single, sharp boundary.) 

troposphere
  The lowest layer of Earth's atmosphere, extending from the surface vertically upwards to around 10-15 km.

  Earth's "weather layer": virtually all of Earth's clouds, precipitation, and movements of mass within the atmosphere occur within the troposphere.

  Within the troposphere, the {term}`lapse rate` is generally positive: temperatures *decrease* with height, globally averaged by around 6 Kelvin per kilometer.

  Earth's {term}`emission height` of around 5-6 km sits within the troposphere.

  Vertically above the troposphere is the *stratosphere*.

two-band approximation
  The commonly used simplification of the spectral dependence of radiative transfer for Earth's climate where all radiation from the sun arriving at Earth is considered {term}`shortwave radiation` (SW) and all radiation emitted by the Earth is considered {term}`longwave radiation` (LW).

typhoon
  Another name for a {term}`tropical cyclone`, specifically for those storms that form in the western Pacific in the Northern Hemisphere that affect places like the Phillipines and Southeast Asia.

water vapor feedback
  The {term}`radiative feedback` due to the increase of atmospheric water vapor with temperature, which is driven most fundamentally by the {term}`Clausius-Clapeyron` equation.  Because water vapor is a potent {term}`greenhouse gas`, the resulting increase in the {term}`absorption` of {term}`longwave radiation` acts to amplify the initial {term}`radiative forcing` that led to the initial temperature change.  It is therefore a {term}`positive feedback`.

wave-particle duality
  From quantum mechanics, the fact that electromagnetic radiation acts as if, on the one hand, it consisted of discrete, individual particles, which we call {term}`photon`s, but simultaneously, on the other hand, acts as if instead it is a continuous wave, characterized by its **wavelength**, **frequency**, or **wavenumber**.

  This enables us to pick and choose whichever perspective is most helpful to the given problem at hand.  For example, when thinking about the {term}`absorption` of EM radiation when it hits a molecule, it is easiest to conceptualize this as individual {term}`photon`s hitting the molecule and exciting the molecule to a higher energetic state, with the photon being annhilated in the process.

  Conversely, when thinking about the energy content of EM radiation, this is most succinctly expressed in terms of its wave properties, namely $E=h\nu$, where $E$ is energy in Joules, $h$ is **Planck's constant**, and $\nu$ is the EM wave's **frequency**

work
  In physics, **force** times the distance over which that force is applied: $w=Fd$, where $w$ is work, $F$ is the force, and $d$ is the distance.  
  
  Physical dimensions: since force has dimensions mass $\times$ length / time$^2$, work must have dimensions mass $\times$ length$^2$ / time$^2$.  These are the same dimensions as energy, and thus the SI units are Joules.

  For us, it comes up most directly when thinking about {term}`tropical cyclone`s as {term}`Carnot cycle`s.

  For more: [Wikipedia page](https://en.wikipedia.org/wiki/Work_(thermodynamics))
```

<!-- grease ice
  
pancake ice

melt pond

halocline

detection

Anki
  For more: [Anki official website](https://apps.ankiweb.net/); [Michael Nielsen's 2018 article, "Augmenting Long-term Memory"](https://augmentingcognition.com/ltm.html)

attribution

historical run

frazil ice
  Ice crystals of roughly a millimeter in size suspended in liquid water.  They are what forms in the initial phase of sea ice growth.  [Wikipedia page](https://en.wikipedia.org/wiki/Frazil_ice)

future projection

forgetting curve
  For more: forgetting curve [Wikipedia page](https://en.m.wikipedia.org/wiki/Forgetting_curve)

spaced repetition
  For more: [Wiki](https://en.m.wikipedia.org/wiki/Spaced_repetition) -->
