# Realistic-Depth Knothe Spread Grid (PLACEHOLDER Grid; SYNTHETIC / SIMULATION)

> **SYNTHETIC / SIMULATION** — Literature-basis sensitivity checks on frozen v3 models; nothing here is validated on real data.

| cell_id | H (m) | tan(beta) | R = H/tan(beta) (m) | sigma (m) | sigma (network radii, R_net=14.14m) | Above 1.5-radius main cap? |
|---|---:|---:|---:|---:|---:|---|
| `H50_tanB1p5` | 50 | 1.5 | 33.33 | **13.30** | **0.940** | NO (<=1.5, in main range) |
| `H50_tanB2p0` | 50 | 2.0 | 25.00 | **9.97** | **0.705** | NO (<=1.5, in main range) |
| `H50_tanB2p5` | 50 | 2.5 | 20.00 | **7.98** | **0.564** | NO (<=1.5, in main range) |
| `H100_tanB1p5` | 100 | 1.5 | 66.67 | **26.60** | **1.881** | YES (simulated) |
| `H100_tanB2p0` | 100 | 2.0 | 50.00 | **19.95** | **1.411** | NO (<=1.5, in main range) |
| `H100_tanB2p5` | 100 | 2.5 | 40.00 | **15.96** | **1.128** | NO (<=1.5, in main range) |
| `H200_tanB1p5` | 200 | 1.5 | 133.33 | **53.19** | **3.761** | YES (simulated) |
| `H200_tanB2p0` | 200 | 2.0 | 100.00 | **39.89** | **2.821** | YES (simulated) |
| `H200_tanB2p5` | 200 | 2.5 | 80.00 | **31.92** | **2.257** | YES (simulated) |
| `H300_tanB1p5` | 300 | 1.5 | 200.00 | **79.79** | **5.642** | YES (simulated) |
| `H300_tanB2p0` | 300 | 2.0 | 150.00 | **59.84** | **4.231** | YES (simulated) |
| `H300_tanB2p5` | 300 | 2.5 | 120.00 | **47.87** | **3.385** | YES (simulated) |
