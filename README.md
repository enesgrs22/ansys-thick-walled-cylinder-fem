# Thick-Walled Cylinder FEM Analysis using ANSYS APDL

This project presents a finite element analysis of a thick-walled
cylinder subjected to uniform internal pressure.

A 2D axisymmetric model was developed in ANSYS Mechanical APDL
using PLANE182 elements. The finite element results were validated
against the classical analytical Lamé solution.

## Objectives

- Develop a 2D axisymmetric finite element model
- Investigate mesh convergence
- Evaluate radial displacement
- Evaluate radial and hoop stress distributions
- Extract results along the cylinder wall thickness
- Compare FEM results with the analytical Lamé solution

## Model Parameters

| Parameter | Value |
|---|---:|
| Inner radius | 58 mm |
| Outer radius | 113 mm |
| Internal pressure | 53 MPa |
| Young's modulus | 200 GPa |
| Poisson's ratio | 0.30 |

## Mesh Refinement

| Mesh | Elements | Nodes |
|---|---:|---:|
| Coarse | 320 | 369 |
| Medium | 1280 | 1377 |
| Fine | 6000 | 6231 |

## Validation

The fine mesh results showed very close agreement with the
analytical Lamé solution.

At the inner surface:

| Quantity | FEM | Analytical |
|---|---:|---:|
| Radial stress | -51.515 MPa | -53.000 MPa |
| Hoop stress | 90.160 MPa | 90.914 MPa |
| Radial displacement | 30.974 μm | 30.976 μm |

The radial displacement shows almost exact agreement with the
analytical solution, while the radial stress difference at the
inner boundary is approximately 2.8%.

## IMAGES
<img width="860" height="970" alt="image" src="https://github.com/user-attachments/assets/49be77d6-9cb4-4e51-a8cc-ae7c4baf2a71" />
<img width="811" height="604" alt="image" src="https://github.com/user-attachments/assets/30af0791-61a6-4e64-aa49-7fa1cc254ee8" />
<img width="844" height="639" alt="image" src="https://github.com/user-attachments/assets/ac7a76b4-dde7-4f4b-a873-8496513059a5" />
<img width="788" height="592" alt="image" src="https://github.com/user-attachments/assets/0d2b25af-b506-4b73-a289-d768981477f1" />
<img width="731" height="664" alt="image" src="https://github.com/user-attachments/assets/23a221d7-f474-4cd9-adca-e7ddbccfa7c1" />
<img width="664" height="610" alt="image" src="https://github.com/user-attachments/assets/552847d4-a6d2-49f8-81b7-28d93b5e88b5" />
<img width="658" height="604" alt="image" src="https://github.com/user-attachments/assets/7cdbbdd8-3592-4187-9040-df7212799b95" />
<img width="720" height="439" alt="image" src="https://github.com/user-attachments/assets/d5608bb4-d329-4a13-9f3d-455223f741e7" />
<img width="722" height="441" alt="image" src="https://github.com/user-attachments/assets/db371a24-7184-4740-80dd-952c63d46372" />
<img width="715" height="443" alt="image" src="https://github.com/user-attachments/assets/ab0c5e76-d91d-4b69-8271-0ecc7ba12d30" />
<img width="731" height="447" alt="image" src="https://github.com/user-attachments/assets/4318371e-da3d-48b5-8f13-6fff5d04904d" />

## Tools

- ANSYS Mechanical APDL
- Finite Element Method
- PLANE182 Axisymmetric Elements
- Analytical Lamé Solution
