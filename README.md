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

