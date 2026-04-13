# Aviation Accident Analysis

**Client:** Airline/Airplane Insurer  
**Data:** NTSB Aviation Accident Database, 1948–2023  
**Scope:** Professional-build airplanes, 1983–2023 (40-year active-model window), 17,205 accidents after cleaning

---

## Project Summary

This analysis identifies the safest aircraft makes and models in the event of an accident, measured by:
- **Serious/Fatal Injury Rate:** fraction of occupants fatally or seriously injured
- **Destruction Rate:** fraction of accidents resulting in total aircraft loss

Separate recommendations are provided for **small aircraft (≤20 aboard)** and **large aircraft (>20 aboard)**.

---

## Key Findings

### Recommended Makes

| Category | Make | Mean Injury Rate | N Accidents |
|---|---|---|---|
| Large | Boeing | 5.7% | 548 |
| Large | McDonnell Douglas | 0.8% | 53 |
| Small | Cessna | 26.5% | 7,068 |
| Small | Maule | 16.5% | 215 |

### Top Recommended Models

**Large Aircraft:**

| Model | Mean Injury Rate | Destruction Rate | N |
|---|---|---|---|
| Boeing 777 | 0.08% | 6.3% | 33 |
| Boeing 757 | 0.15% | 0.0% | 18 |
| Boeing 787 | 0.31% | 0.0% | 11 |
| Boeing 737-7H4 | 0.32% | 0.0% | 12 |
| Bombardier CL-600-2B19 | 0.44% | 0.0% | 14 |

**Small Aircraft:**

| Model | Mean Injury Rate | Destruction Rate | N |
|---|---|---|---|
| Cessna 172SP | 0.0% | 0.0% | 12 |
| Diamond DA 20 C1 | 0.0% | 0.0% | 11 |
| Cessna 180H | 4.9% | 0.0% | 34 |
| Cessna 195 | 5.0% | 0.0% | 37 |

---

## Contributing Factors

### Factor 1: Weather Conditions (VMC vs IMC)

Accidents in **Instrument Meteorological Conditions (IMC)** produce dramatically worse outcomes:
- Mean injury rate: **62.7% (IMC)** vs **23.4% (VMC)**
- Destruction rate: **37.3% (IMC)** vs **7.3% (VMC)**

This is a nearly 3× multiplier on injury severity and 5× on destruction. Sample sizes are large (n=14,324 VMC; n=900 IMC), making this a highly robust finding.

![Weather Factor](figures/fig8_weather.png)

### Factor 2: Engine Type

**Turbofan** engines are associated with the lowest accident severity:
- Mean injury rate: **8.8%** — roughly 3× lower than reciprocating/piston engines (25.5%)
- Destruction rate: **9.7%** — lowest of all engine types
- Turboprop engines show the highest injury rate (32.1%), likely reflecting remote-operations exposure

![Engine Type Factor](figures/fig9_engines.png)

---

## Visualisations

| Figure | Description |
|---|---|
| fig1_accidents_over_time | Accident frequency trend 1983–2023 |
| fig2_makes_injury_rate | Top 15 makes by injury rate (small & large) |
| fig3_violin_small | Injury rate distribution — top 10 small makes |
| fig4_strip_large | Individual injury rates — top 10 large makes |
| fig5_destruction_rate | Destruction rate by make (small & large) |
| fig6_models_large | Top 15 large aircraft models by injury rate |
| fig7_models_small | Top 15 small aircraft models by injury rate |
| fig8_weather | Outcomes by weather condition |
| fig9_engines | Outcomes by engine type |

---


