- G1 Add: 0.75x
- G1 Mul: No change
- G1 MSM: 2.5x
- Map to G1: 0.75x
- G2 Add: 0.75x
- G2 Mul: 0.5x
- G2 MSM: 4x (so 2x overall with change to mul)
- Map to G2: 0.2x
- Pairing: 1.2x

This corresponds to the following gas prices:
```
GAS_COST_g1add-1=375
GAS_COST_g1mul-1=12000
GAS_COST_g2add-1=600
GAS_COST_g2mul-1=22500
GAS_COST_mapfp-1=4125
GAS_COST_mapfp2-1=15000
GAS_COST_PAIRING_m=51600
GAS_COST_PAIRING_c=78000
GAS_G1_MSM_MULTIPLIER=400
GAS_G2_MSM_MULTIPLIER=250
```

EcRecover runs at about 80mgas/s on NUC.
This would give following NUC results:
```
g1add-1: 86.61 mgas/s (83.42-90.05)
g1mul-1: 86.90 mgas/s (83.24-90.89)
g2add-1: 82.34 mgas/s (78.50-86.58)
g2mul-1: 93.40 mgas/s (88.11-99.38)
mapfp2-1: 104.4 mgas/s (104.0-104.9)
mapfp-1: 89.96 mgas/s (85.91-94.40)
g1msm-1: 265.0 mgas/s (258.9-271.5)
g1msm-10: 151.8 mgas/s (151.4-152.2)
g1msm-11: 145.7 mgas/s (145.4-146.1)
g1msm-12: 139.8 mgas/s (136.0-143.8)
g1msm-128: 83.04 mgas/s (82.57-83.51)
g1msm-13: 136.9 mgas/s (136.1-137.6)
g1msm-14: 132.8 mgas/s (132.2-133.3)
g1msm-15: 119.6 mgas/s (114.5-125.1)
g1msm-16: 112.9 mgas/s (108.7-117.5)
g1msm-17: 117.1 mgas/s (116.8-117.5)
g1msm-18: 117.1 mgas/s (116.6-117.5)
g1msm-19: 110.7 mgas/s (107.1-114.5)
g1msm-2: 205.1 mgas/s (199.2-211.4)
g1msm-20: 117.4 mgas/s (117.0-117.8)
g1msm-2048: 90.14 mgas/s (88.20-92.17)
g1msm-21: 113.4 mgas/s (110.2-116.9)
g1msm-22: 109.8 mgas/s (106.2-113.7)
g1msm-23: 113.6 mgas/s (113.2-114.0)
g1msm-24: 107.4 mgas/s (103.7-111.4)
g1msm-25: 111.6 mgas/s (111.2-111.9)
g1msm-256: 86.62 mgas/s (85.96-87.29)
g1msm-26: 105.5 mgas/s (101.5-109.7)
g1msm-27: 109.7 mgas/s (109.4-110.1)
g1msm-28: 103.2 mgas/s (99.68-106.9)
g1msm-29: 106.9 mgas/s (106.5-107.4)
g1msm-3: 193.4 mgas/s (190.5-196.4)
g1msm-30: 101.1 mgas/s (97.83-104.6)
g1msm-31: 105.2 mgas/s (104.7-105.7)
g1msm-32: 102.4 mgas/s (101.8-102.9)
g1msm-4: 184.6 mgas/s (178.2-191.5)
g1msm-4096: 93.82 mgas/s (90.39-97.51)
g1msm-5: 178.5 mgas/s (172.1-185.4)
g1msm-512: 90.21 mgas/s (89.74-90.70)
g1msm-6: 158.2 mgas/s (156.8-159.6)
g1msm-64: 86.09 mgas/s (82.11-90.48)
g1msm-7: 159.4 mgas/s (154.2-165.0)
g1msm-8: 153.4 mgas/s (153.3-153.5)
g1msm-9: 140.1 mgas/s (133.8-147.2)
g2msm-1: 248.3 mgas/s (228.6-271.6)
g2msm-10: 126.0 mgas/s (115.4-138.7)
g2msm-11: 116.8 mgas/s (104.3-132.8)
g2msm-12: 119.1 mgas/s (109.6-130.5)
g2msm-128: 75.06 mgas/s (67.88-83.93)
g2msm-13: 112.8 mgas/s (102.8-125.0)
g2msm-14: 104.6 mgas/s (94.88-116.5)
g2msm-15: 105.5 mgas/s (92.96-122.1)
g2msm-16: 109.1 mgas/s (98.16-122.8)
g2msm-17: 97.04 mgas/s (87.73-108.6)
g2msm-18: 108.2 mgas/s (99.68-118.4)
g2msm-19: 100.5 mgas/s (90.35-113.1)
g2msm-2: 185.7 mgas/s (168.9-206.3)
g2msm-20: 106.9 mgas/s (97.29-118.7)
g2msm-2048: 96.32 mgas/s (86.31-109.0)
g2msm-21: 106.5 mgas/s (96.72-118.5)
g2msm-22: 107.8 mgas/s (96.11-122.7)
g2msm-23: 94.72 mgas/s (87.03-103.9)
g2msm-24: 101.9 mgas/s (95.29-109.4)
g2msm-25: 94.65 mgas/s (84.80-107.1)
g2msm-256: 80.92 mgas/s (71.32-93.50)
g2msm-26: 96.59 mgas/s (86.76-108.9)
g2msm-27: 97.09 mgas/s (86.79-110.2)
g2msm-28: 99.22 mgas/s (92.10-107.5)
g2msm-29: 95.41 mgas/s (88.14-104.0)
g2msm-3: 177.2 mgas/s (162.7-194.5)
g2msm-30: 96.92 mgas/s (87.77-108.2)
g2msm-31: 93.81 mgas/s (89.56-98.48)
g2msm-32: 102.1 mgas/s (93.50-112.5)
g2msm-4: 159.2 mgas/s (148.4-171.7)
g2msm-4096: 104.1 mgas/s (95.68-114.1)
g2msm-5: 160.7 mgas/s (152.6-169.8)
g2msm-512: 89.00 mgas/s (82.91-96.05)
g2msm-6: 146.1 mgas/s (136.1-157.6)
g2msm-64: 85.75 mgas/s (79.90-92.52)
g2msm-7: 148.3 mgas/s (133.9-166.2)
g2msm-8: 133.4 mgas/s (122.6-146.2)
g2msm-9: 129.7 mgas/s (119.9-141.1)
pairing-1: 98.17 mgas/s (86.76-113.0)
pairing-2: 97.18 mgas/s (89.10-106.9)
pairing-3: 92.61 mgas/s (85.50-101.0)
pairing-4: 89.95 mgas/s (83.19-97.91)
pairing-5: 89.82 mgas/s (81.84-99.52)
pairing-6: 86.38 mgas/s (78.36-96.24)
pairing-7: 89.62 mgas/s (82.97-97.43)
pairing-8: 82.44 mgas/s (75.68-90.53)
```