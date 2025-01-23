# Nitrate_Photolysis_Aqueous_Solution
Data and supplementary information of manuscript ["Revealing Photochemical Pathways of Nitrate in Water through First-Principles Simulations"](https://chemrxiv.org/engage/chemrxiv/article-details/67769779fa469535b98bbb25).

<p align="center">
<img src="Nitrate_Photolysis_Solution_ToC.png" width="450">
</p>

This repository has the following directories:
- Gas-Phase:
    - nitrate_cam-b3lyp_scan.inp: The [ORCA](https://orcaforum.kofo.mpg.de/app.php/portal) input file to perform a potential energy surface scan at the ground state of nitrate at the level of CAM-B3LYP.
    - guess_template.inp: The ORCA input file to generate quasi-restricted orbitals as the initial guess for multi-reference calculations.
    - sa-casscf_template.inp: The ORCA input file to perform SA-CASSCF calculations.
    - nevpt2_template.inp: The ORCA input file to perform NEVPT2 calculations.
    - mrci+q_template.inp: The ORCA input file to perform MRCI+Q calculations.
    - nitrate_revpbe0_scan.inp: The ORCA input file to perform a potential energy surface scan at the ground state of nitrate at the level of revPBE0.
    - nitrate_t1_revpbe0_template.inp: The ORCA input file to perform vertical excitations to the first triplet state of nitrate at the level of revPBE0.

- S0_MD:
    - cp2k.inp: The [CP2K](https://manual.cp2k.org/trunk/#gsc.tab=0) input file to perform AIMD simulations at the ground state of nitrate.
    - nh4no3_63h2o_pbe.xyz: The initial configuration for the AIMD simulations at the ground state.

- UV_Vis:
    - orca_template.inp: The ORCA input file to perform TD-DFT calculations to generate the UV-Visible absorption spectra.
 
- T1_MD:
    - cp2k.inp: The CP2K input file to perform AIMD simulations at the triplet state of nitrate.
    - nh4no3_63h2o_revpbe0.xyz: The initial configuration for the AIMD simulations at the triplet state.
 
- T1_MetaD:
    - cp2k.inp: The CP2K input file to perform AIMD simulations with metadynamics at the triplet state of nitrate.
    - plumed.dat: The [PLUMED](https://www.plumed.org/doc-v2.9/user-doc/html/index.html) input file to define parameters for metadynamics simulations.
    - COLVAR files: The PLUMED output files containing the CVs and applied biases along the simulation.
    - HILLS files: The PLUMED output files containing the applied Gaussians along the simulation.
    - XYZ files: The initial configurations.
    - walker-0: The directory for walker-0 in the multiple-walkers metadynamics simulation.
    - walker-1: The directory for walker-1 in the multiple-walkers metadynamics simulation.
    - hills: The input files and data for reproducing Figure 4 and S7.
