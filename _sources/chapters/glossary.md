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

aerosol
  A small solid particle in the atmosphere.  There are naturally occuring aerosols such as sea salt and dust.  There are also {term}`anthropogenic` aerosols such as sulfate and smoke from combustion.

  Thir precise radiative properties varies a lot across aerosol species.
  
  With respect to historical emissions of aerosols by humans, overall they have slightly increased the planetary {term}`albedo` by directly {term}`scattering` {term}`shortwave radiation` back to space, which constitutes a negative {term}`radiative forcing`.

  They have contributed an even more negative---but highly uncertain---negative radiative forcing through their influence on cloud {term}`albedo` via their role as cloud condensation nuclei.

albedo
  The fraction of the sun's radiation that is reflected back to space.  It is a dimensionless quantity and thus unitless.  Usually denoted with a Greek lower-case alpha, $\alpha$.
  
  The *planetary* albedo, meaning the global-mean, time-mean value of the albedo at the {term}`top of atmosphere` is often denoted $\alpha_p$ and for Earth's present climate is approximately 0.3: approximately 30% of the insolation is reflected back to space, meaning that remaining 0.7 or 70% is absorbed within the climate system.

  It turns out that within Earth's climate system there is very little reflection of {term}`longwave radiation`, which is why albedo is only associated with shortwave radiation.

  (Technically, albedo is a *spectral* property: the precise albedo of a given material depends on the precise wavelength of the radiation incident on that material, not just the bulk SW vs. LW.  So, formally, $\alpha=\alpha(\lambda)$.  But in the {term}`two-stream approximation`, we treat it as being a bulk property of just the {term}`shortwave radiation`,)

anthropogenic
  A fancy term for *caused by humans*.  As opposed to *natural*, *naturally occuring*, etc.  So, for example, we can distinguish between *natural climate changes* on the one hand (as occur, say, between the ice ages and interglacial periods due to the planet's naturally occuring orbital fluctuations), with, on the other hand, *anthropogenic climate change* which is the set of ongoing changes to Earth's climate caused by human activities.

blackbody
  A body that emits electromagnetic radiation according to the {term}`Stefan-Boltzmann law`.  The sun and Earth's surface can be approximated as perfect blackbodies, whereas Earth's atmosphere is an imperfect blackbody, meaning it has an {term}`emissivity` that is less than one.

climate model
  A representation of Earth's climate system on a computer, usually a supercomputer.  Traditionally, they work by chunking the ocean, atmosphere, and land into lots of small *gridboxes* (though the shapes aren't always a simple box) and solving the equations of motion, equations of radiative transfer, and equations representing other key processes forward in time.

  The laws of nature and the real Earth are *continuous*, whereas a computer treats things as *discrete*: climate model gridboxes have finite sizes, and the climate model advances forward in time in discrete finite chunks, e.g. 30 minutes per *timestep*.  This creates all sorts of biases and uncertainties.

Clausius-Clapeyron
  The equation from thermodynamics that gives rise to the roughly exponential increase in saturation specific humidity with warming, at a rate of approximately $7\%\text{ K}^{-1}$.   

  Insofar as the {term}`relative humidity` stays fixed, this 7% increase per Kelvin warming extends to the specific humidity too.  But note that changes in *relative* humidity---or lack thereof---are *not* directly determined by Clausius-Clapeyron.
  
  (More formally, the Clausius-Clapeyron equation specifies the dependence of saturation vapor pressure on temperature: $d\ln e^*/dT=L_v/(R_vT^2)$, where $e^*$ is saturation vapor pressure, $T$ is temperature, $L_v=2.5\times10^6\text{ J kg}^{-1}$ is the latent heat of vaporization, and $R_v=461.5\text{ J kg}^{-1}\text{ K}^{-1}$ is the specific gas constant of water vapor.  Plugging those values of $L_v$ and $R_v$ in and using temperature ranges within the troposphere, so $T\sim200$ to $300\text{ K}$, yields the approximate $7\%\text{ K}^{-1}$ scaling.)

climate sensitivity
  The global-mean surface temperature change caused by a doubling of atmospheric CO$_2$ concentration.  Units Kelvin or degrees Celsius.  
  
  There are two meaningful variants: {term}`equilibrium climate sensitivity` and {term}`transient climate sensitivity`, which differ based on the *timescale* considered.

  This cannot be directly observed: we don't have a 2nd Earth available where we can instantly double ${\text{CO}_2}$ and then watch equilibrate over thousands of years.  It therefore must be estimated using climate models.

cloud feedback
  The {term}`radiative feedback` due to changes in cloud properties.

  These are highly uncertain, due to the large number of processes involved and the vast range of underlying physical scales, from micron-scale changes in e.g. cloud droplet size that influence cloud {term}`albedo` all the way up to changes in planetary-scale flow patterns that influence the overall location, extent, and height of different cloud types.

  That said, the current best estimate of the global-mean cloud feedback is that it is a mildly {term}`positive feedback`.

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

equilibrium climate sensitivity
  The {term}`climate sensitivity` after the whole climate system, including the deep ocean, reaches a new equilibrium state.  Because heat transfer within the deep ocean is very slow, this takes thousands of years.

greenhouse gas
  A molecule in Earth's atmosphere that significantly absorbs {term}`longwave radiation`.  The two most important ones are carbon dioxide (CO$_2$) and water vapor (H$_2$O).  Others include methane (CH$_4$), nitrous oxide (N$_2$O), and ozone (O$_3$)

insolation
  A contraction of the phrase "**in**coming **sol**ar radi**ation**": the amount of solar radiation incident at Earth's {term}`top of atmosphere`.  Physical dimensions are power per area; SI units are Watts divided by square meter, $\text{W m}^{-2}$.

internal variability
  A.k.a. "natural variability."  The naturally occuring ~random-ish fluctuations that occur on many different timescales in Earth's atmosphere and ocean.  Even for global-mean surface temperature, such internal variability can result in several years or even multiple decades of warming or cooling.

  That is even more the case when considering smaller scales.  In general, the smaller the timescale and/or spatial scale, the greater influence internal variability will have on the behavior relative to other factors.

Kelvin
  Absolute temperature, such that zero Kelvin equals [absolute zero](https://en.wikipedia.org/wiki/Absolute_zero).  Abbreviated K.  The SI unit for temperature.  Equal to degrees Celsius plus 273.15.  

  Because it has the identical *spacing* as degrees Celsius, for quantities that represent *differences* in temperature the two units can be used interchangeably.  For example, when we say the planet warms up by a given amount, that refers to the new temperature *minus* the old temperature, and so it is the same number in Kelvin as degrees Celsius.

  Conversely, if we were talking about Earth's current global-mean temperature, which is approximately 288 Kelvin, that is **not** the same as $288^\circ\text{C}$.  It *is* the same as $288-273.15=14.85^\circ\text{C}$.
  
  Another example, we can say that the average {term}`lapse rate` in the troposphere is approximately 6 Kelvin per kilometer, or just as well that it is 6 degrees Celsius per kilometer.  That's because the lapse rate is the *change* in temperature with height, i.e. the (infinitesimal) difference in temperature between two adjacent heights.

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

outgoing longwave radiation
  The upward flux of longwave radiation at the top of the atmosphere, in units Watts divided by square meter, $\text{W m}^{-2}$.  Commonly abbreviated to OLR.  *Outgoing* means that it is signed positive out of the atmosphere.  The global-mean value at present is roughly $240\text{W m}^{-2}$.

Planck feedback
  The {term}`radiative feedback` stemming directly from the {term}`Stefan-Boltzmann law`: blackbody emission increases with temperature to the fourth power, and so all else equal if the surface temperature and rest of the troposphere warm up by some amount, the {term}`outgoing longwave radiation` will increase, acting to reduce the net imbalance at the {term}`top of atmosphere` that led to the initial warming.

  Globally averaged, it is the single largest {term}`negative feedback`.

  Regionally, it contributes to {term}`polar amplification` because the increase in radiation per unit warming itself increases with the original temperature.  As such, warming in the Tropics---where it's already warm---leads to a larger increase in emitted {term}`longwave radiation` compared to the same warming near the poles where, compared to the Tropics, it's much colder.

polar amplification
  The tendency for surface temperature increases in response to positive {term}`radiative forcing` such as increased CO$_2$ to be greater near the poles than at lower latitudes.  This is especially true for the Arctic, and so sometimes it's referred to as *Arctic amplification*.  
  
  There are three key {term}`radiative feedback` processes that contribute to polar amplification, in each case due to that feedback being more stabilizing at lower latitudes than at higher latitudes: (1) {term}`Planck feedback`, (2) {term}`surface albedo feedback`, and (3) {term}`lapse rate feedback`

  For the Antarctic, the prevailing upwelling of cold water from depth in the Southern Ocean tends to delay the warming in the southern high latitudes.

positive feedback
  For our purposes, a {term}`radiative feedback` that acts to *amplify* an existing radiative *imbalance* at the {term}`top of atmosphere`.  A.k.a. an *amplifying* feedback.  As such, positive feedbacks act to amplify suface warming.

  For the global mean, the key positive feedbacks are the {term}`water vapor feedback` and {term}`surface albedo feedback`.  The {term}`cloud feedback` is most likely positive too, but it is subject to much more uncertainty.

  Note: in response to a *negative* {term}`radiative forcing`, the overall surface air temperature response will be negative, i.e. cooling.  In that case, a "positive" feedback *amplifies* the temperature change, i.e. contributes *more* cooling, not less.  (That's why the "positive" vs. "negative" terms are a little confusing compared to "amplifying" vs. "inhibiting".)

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

shortwave radiation
  Essentially, the radiation emitted by the Sun.  This corresponds to electromagnetic radiation with wavelengths spanning approximately 0.1-2 {term}`micron`.  Commonly abbreviated to SW.  Units are Watts divided by square meter, $\text{W m}^{-2}$.

  To be contrasted with {term}`longwave radiation`, which essentially is the radiation emitted by the Earth.

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

surface albedo feedback
  In response to a positive {term}`radiative forcing` (such as increased CO$_2$), surface temperatures increase, causing some ice and snow will melt, which exposes darker ocean or land surface underneath and thus causes more {term}`shortwave radiation` to be absorbed.  This acts to increase the original positive radiative forcing and thus amplify the warming, compared to the hypothetical case if the surface albedo had remained unchanged.  It thus constitutes a {term}`positive feedback` in the global mean.

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

tropopause
  The boundary between the {term}`troposphere` and {term}`stratosphere`.  Typically around 10-15 km, with the higher values generally in the tropics and lower values in the extratropics.

  (Although we often treat it as a single height or pressure, in reality there is some finite-depth transition region between the troposphere and stratosphere, and even the position and depth of that transition layer can vary depending on the precise definition used.  But it is still very useful for us in this course to treat it as being a single, sharp boundary.) 

troposphere
  The lowest layer of Earth's atmosphere, extending from the surface vertically upwards to around 10-15 km.

  Earth's "weather layer": virtually all of Earth's clouds, precipitation, and movements of mass within the atmosphere occur within the troposphere.

  Within the troposphere, the {term}`lapse rate` is generally positive: temperatures *decrease* with height, globally averaged by around 6 Kelvin per kilometer.

  Earth's {term}`emission height` of around 5-6 km sits within the troposphere.

  Vertically above the troposphere is the *stratosphere*.

two-stream approximation
  The commonly used simplification of the spectral dependence of radiative transfer for Earth's climate where all radiation from the sun arriving at Earth is considered {term}`shortwave radiation` (SW) and all radiation emitted by the Earth is considered {term}`longwave radiation` (LW).

water vapor feedback
  The {term}`radiative feedback` due to the increase of atmospheric water vapor with temperature, which is driven most fundamentally by the {term}`Clausius-Clapeyron` equation.  Because water vapor is a potent {term}`greenhouse gas`, the resulting increase in the {term}`absorption` of {term}`longwave radiation` acts to amplify the initial {term}`radiative forcing` that led to the initial temperature change.  It is therefore a {term}`positive feedback`.
```
