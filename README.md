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

## Tools

- ANSYS Mechanical APDL
- Finite Element Method
- PLANE182 Axisymmetric Elements
- Analytical Lamé Solution
