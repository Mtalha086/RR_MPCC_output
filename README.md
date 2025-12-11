# RR_MPCC_output

MPCC Scans and Error Analysis — Repository Guide

This repository contains numerical results for MPCC/CC2 scans across multiple basis sets and molecules.
The structure is designed to make navigation clear and consistent.

Repository Structure

At the top level, the repository contains four basis-set directories:

cc-pvdz/
cc-pvtz/
aug-cc-pvdz/
aug-cc-pvtz/

Each basis directory contains subfolders corresponding to molecules, for example:

cc-pvdz/
    TIP4P-6/
    C6H14/
    ...

Contents of Each Molecule Folder

Within each molecule directory, results are organized by scan type.
The four scan types included are:

Lov

Lvv

Lov_Lvv_fix_Loo_1

Lvv_fix_Loo_1

For each scan, the following folders are present:

energies_folder_{scan}

CC2 energy convergence plots

Shows iteration-wise energy behavior

Y_amp_{scan}

L2 error of Y amplitudes

Histogram of Y amplitude distribution

Omega_{scan}

L2 error of Ω

Histogram of Ω distribution

Foo_{scan}

L2 error of Fₒₒ

Histogram

Fov_{scan}

L2 error of Fₒᵥ

Histogram

Fvv_{scan}

L2 error of Fᵥᵥ

Histogram

Combined 2×2 Plots

For convenience, summary 2×2 plots (CC2 convergence + L2 errors for Y and Ω) are stored in:

RR_MPCC_output/


Notes

All results in this repository currently use tol = 1e-4 unless stated otherwise.
