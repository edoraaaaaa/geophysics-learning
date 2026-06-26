bash
cat > /mnt/user-data/outputs/02-earth-internal-heat.md << 'EOF'
# Earth's Internal Heat

## Learning Objectives

By the end of this section, you should be able to:
- Quantify the two primary sources of Earth's internal heat and their relative contributions
- Explain radioactive decay as a heat-generating mechanism in crustal rocks
- Describe how heat flows from Earth's interior to the surface
- Calculate simple heat flow estimates from thermal conductivity and gradient data
- Understand why some regions have anomalously high surface heat flux

---

## 1. Total Heat Budget of Earth

Earth is not in thermal equilibrium — it continuously loses heat to space at a rate of approximately **44–47 terawatts (TW)**. For reference, global human energy consumption is ~18 TW. Earth radiates roughly **2.5× more energy** than humanity currently uses.

| Parameter | Value |
|-----------|-------|
| Total heat flow from Earth | ~44–47 TW |
| Average surface heat flux (continents) | ~65 mW/m² |
| Average surface heat flux (oceans) | ~101 mW/m² |
| Global average surface heat flux | ~87 mW/m² |
| Human global energy consumption | ~18 TW |

The difference between continental and oceanic heat flux is significant: oceanic crust is thinner, younger, and sits closer to convecting mantle, allowing more heat to escape.

---

## 2. Heat Source 1 — Primordial Heat (~50%)

When Earth formed ~4.54 billion years ago, two processes released enormous amounts of energy that are still slowly escaping today:

### 2.1 Accretion

Planetesimals (small rocky bodies) collided and merged to form proto-Earth. Each collision converted kinetic energy into heat. The total energy released:

$$E_{accretion} \approx \frac{3GM_{Earth}^2}{5R_{Earth}} \approx 2.5 \times 10^{31} \text{ J}$$

This is enough energy to completely melt Earth multiple times over. Most was radiated to space during formation, but a significant fraction was trapped inside.

### 2.2 Core Formation (Differentiation)

As proto-Earth grew large enough for internal melting, dense iron and nickel sank to form the core while lighter silicates rose to form the mantle. This gravitational separation released additional energy:

$$E_{differentiation} \approx 1.5–2.5 \times 10^{31} \text{ J}$$

The core, formed ~4.5 billion years ago, is still cooling. The **inner core is solidifying** — latent heat released during this solidification contributes ~0.3–0.5 TW of heat flow today.

### 2.3 Why Is Primordial Heat Still Present?

Rock is an excellent thermal insulator. Earth's thermal diffusivity is extremely low:

$$\kappa = \frac{\lambda}{\rho c_p} \approx 10^{-6} \text{ m}^2/\text{s}$$

The **thermal diffusion timescale** for Earth's radius:

$$t_{diff} = \frac{R_{Earth}^2}{\kappa} \approx \frac{(6.37 \times 10^6)^2}{10^{-6}} \approx 4 \times 10^{19} \text{ s} \approx 10^{12} \text{ years}$$

This is **~70 times the age of the universe** — pure conduction alone would never cool Earth. Mantle convection accelerates heat loss, but primordial heat is still leaking out after 4.5 billion years.

---

## 3. Heat Source 2 — Radiogenic Heat (~50%)

Radioactive isotopes in Earth's rocks continuously decay, converting nuclear binding energy into heat. This is the **only ongoing heat source** (primordial heat is just stored, not generated).

### 3.1 The Four Major Heat-Producing Isotopes

| Isotope | Half-life (Ga) | Heat production (μW/kg) | Concentration in crust |
|---------|---------------|------------------------|------------------------|
| ²³⁸U | 4.47 | 94.6 | ~2.7 ppm |
| ²³⁵U | 0.70 | 584.0 | ~0.02 ppm |
| ²³²Th | 14.0 | 26.4 | ~10.5 ppm |
| ⁴⁰K | 1.25 | 29.2 | ~2.6% (K total) |

Note: ²³⁵U has very high heat production per kg but extremely low concentration today (it was more important early in Earth's history).

### 3.2 Why These Elements Concentrate in the Crust

During partial melting and magmatic differentiation, U, Th, and K are **incompatible elements** — they do not fit easily into the crystal lattice of common mantle minerals (olivine, pyroxene). They are therefore preferentially expelled into the melt and concentrated in:
- **Continental crust** (especially granites and granodiorites)
- **Felsic volcanic rocks** (rhyolite, dacite)

This is why **continental crust produces more radiogenic heat per unit volume** than the mantle, even though the mantle is much larger.

### 3.3 Radiogenic Heat Production by Rock Type

| Rock type | Heat production (μW/m³) |
|-----------|------------------------|
| Granite | 2.5–4.0 |
| Granodiorite | 1.5–3.0 |
| Basalt | 0.3–0.6 |
| Peridotite (mantle) | 0.01–0.05 |
| Limestone/sandstone | 0.5–1.5 |

This explains why geothermal gradients are higher in **granite-rich regions** — the crust itself is generating significant heat.

### 3.4 Temporal Decay of Radiogenic Heat

Early Earth had much more radiogenic heat because isotopes with shorter half-lives (especially ²³⁵U and ⁴⁰K) were more abundant. Radiogenic heat production ~4.5 Ga ago was **3–4× higher** than today.

$$H(t) = H_0 \cdot e^{-\lambda t}$$

This is why early Earth had more vigorous mantle convection and more intense volcanism — more heat needed to be transported to the surface.

---

## 4. Mantle Convection: The Primary Heat Transport Mechanism

Although rock conducts heat slowly, Earth's mantle behaves as a **viscous fluid** over geological timescales (millions of years). Hot rock near the core-mantle boundary becomes buoyant, rises, cools near the surface, becomes denser, and sinks — creating a convection cell.

### 4.1 Key Parameters

| Parameter | Value |
|-----------|-------|
| Mantle viscosity | ~10²¹ Pa·s (10²¹× more viscous than water) |
| Mantle convection velocity | ~2–10 cm/year (same as plate tectonics speed) |
| Rayleigh number (Ra) | ~10⁶–10⁸ (strongly convecting) |

The **Rayleigh number** determines whether a fluid convects:

$$Ra = \frac{\rho g \alpha \Delta T d^3}{\eta \kappa}$$

For Earth's mantle, Ra >> 1000 (critical value), confirming vigorous convection.

### 4.2 Connection to Plate Tectonics

Mantle convection **drives plate tectonics**, which in turn controls where geothermal resources are located:

- **Mid-ocean ridges:** upwelling mantle → thin crust → very high heat flux (>200 mW/m²)
- **Subduction zones:** descending slab triggers mantle wedge melting → volcanic arcs → high heat flux
- **Hot spots:** mantle plumes pierce through plates → anomalous volcanism (Hawaii, Iceland)
- **Cratons:** old, thick, cold continental roots → very low heat flux (<40 mW/m²)

---

## 5. Measuring Earth's Heat Flow

### 5.1 Fourier's Law of Heat Conduction

The fundamental equation governing conductive heat flow:

$$q = -\lambda \frac{dT}{dz}$$

Where:
- $q$ = heat flux (W/m²)
- $\lambda$ = thermal conductivity (W/m·K)
- $dT/dz$ = temperature gradient (K/m), positive downward

The negative sign means heat flows from hot to cold (down the gradient).

### 5.2 Thermal Conductivity of Common Rocks

| Rock type | λ (W/m·K) |
|-----------|-----------|
| Granite | 2.5–3.5 |
| Basalt | 1.5–2.0 |
| Sandstone (dry) | 1.5–2.5 |
| Sandstone (saturated) | 2.0–4.0 |
| Limestone | 2.5–3.5 |
| Clay/shale | 1.0–2.5 |
| Water | 0.6 |
| Steam | 0.025 |

Note: **saturated rocks conduct heat better than dry rocks** because water has higher conductivity than air. This matters significantly for geothermal reservoir characterization.

### 5.3 Heat Flow Measurement in Practice

In boreholes, heat flow is measured by:
1. **Temperature logging** — measure T at multiple depths
2. **Rock sampling** — measure λ on drill cores in lab
3. **Calculate:** $q = \lambda \times (dT/dz)$

Typical measurement depth: 200–3000 m (must be deep enough to avoid surface temperature fluctuations from climate and seasons, which affect the top ~100 m).

### 5.4 Global Heat Flow Database

The **International Heat Flow Commission (IHFC)** maintains a global database of >38,000 heat flow measurements. Indonesia has relatively sparse coverage — many areas have only 1–3 measurements per 100 km², highlighting the need for geophysical exploration.

---

## 6. Surface Temperature Perturbations

Not all temperature variation with depth reflects the deep geothermal gradient. Several near-surface effects must be corrected:

| Perturbation | Depth affected | Correction method |
|-------------|----------------|-------------------|
| Annual temperature cycle | 0–15 m | Wait for thermal stabilization |
| Long-term climate change | 0–150 m | Borehole paleoclimate analysis |
| Topographic effects | 0–500 m | Numerical terrain correction |
| Groundwater flow | Variable | Hydrogeological modeling |
| Magmatic intrusions | Variable | Age dating + thermal modeling |

For this project, the dataset is designed to represent **stabilized borehole temperatures** below 100 m, where these surface effects are minimal.

---

## Key Takeaways

1. Earth emits **~44 TW** of heat — 2.5× global human energy consumption.
2. Heat comes from two roughly equal sources: **primordial heat** (gravitational energy from Earth's formation) and **radiogenic heat** (ongoing radioactive decay).
3. Rock is an extraordinary thermal insulator — primordial heat is still escaping after **4.5 billion years**.
4. **U, Th, and K** are the main heat-producing isotopes, concentrated in continental crust — especially granites.
5. **Mantle convection**, not conduction, is the dominant heat transport mechanism in Earth's interior.
6. Surface heat flux is measured using **Fourier's Law**: $q = -\lambda (dT/dz)$ — the product of thermal conductivity and temperature gradient.
7. Near-surface temperatures are affected by climate, topography, and groundwater — corrections are needed for accurate geothermal gradient measurements.

---

## References

1. Turcotte, D.L. & Schubert, G. (2014). *Geodynamics* (3rd ed.). Cambridge University Press.
2. Stacey, F.D. & Davis, P.M. (2008). *Physics of the Earth* (4th ed.). Cambridge University Press.
3. Pollack, H.N., Hurter, S.J. & Johnson, J.R. (1993). Heat flow from the Earth's interior: Analysis of the global data set. *Reviews of Geophysics*, 31(3), 267–280.
4. Jaupart, C. & Mareschal, J.C. (2011). *Heat Generation and Transport in the Earth*. Cambridge University Press.
5. Davies, J.H. & Davies, D.R. (2010). Earth's surface heat flux. *Solid Earth*, 1, 5–24. [Open Access]
6. Rudnick, R.L. & Gao, S. (2003). Composition of the continental crust. *Treatise on Geochemistry*, 3, 1–64.
