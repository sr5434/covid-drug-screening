# COVID Drug Screening
This repository screens about 120 drugs to identify candidates for inhibiting the main protease of SARS-CoV-2, which is responsible for cutting polyproteins into usable pieces. The drugs work by getting stuck in the active site of the main protease, disabling it and preventing viral reproduction. Initially, drugs passed through a quick docking stage to identify promising candidates. These candidates moved onto a second, more rigorous evaluation. The best candidates after this more rigorous evaluation were then tested for absorbtion and hepatotoxicity.

This project was created by Samir Rangwalla, Gary Goodson, Neil Bhatt, and Ali Sayed.
## Candidates
Some drugs are known antivirals for COVID 19, and were included in initial candidate pool to verify that the pipeline worked. The following candidates were identified:
 - Ensitrelvir
 - PF00835231
 - Ibuzatrelvir
 - Imatinib
 - NZ-804
 - Olgotrelvir
 - Iscartrelvir
 - Kaempferol

## Scripts
```Docking.ipynb``` and ```Docking_2.ipynb``` effectively do the same thing, and were separated so we could batch the processing of the initial candidate pool. ```Toxicity.ipynb``` analyzes pharmacokinetics, and records CYP inhibition, Lipinski's Rule of 5 violations, and Veber rule violations. It also includes a utility to visualize candidates and see how they fit in the active site. In order to use that notebook, download the files stored in docked_compounds and store them in the same folder as ```Toxicity.ipynb``` (if you are using Google Colab, just upload them to the environment).
