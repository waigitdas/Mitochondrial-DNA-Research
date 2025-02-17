# Haplogroip Assignments
 
Haplogroup assignments were provided by the Mitomap team at Children's Hosdpital of Philadelphia. The used the Haplogrep3 tools. The assignments were added as a propterty to the Genbank sequence nodes. 

This project intended to replicate these assignmentsusing graph methods. That effort failed. The Excel workbooks in this folder Used traversals of the dnode (haplotree) paths from Eve to the assigned haplogroup node. show:

<ol>
 <li>Traversals to the assiggned hapolgroup node were successful foe only 34% of the Genbank sequences.</li>
 <li>The C16189T was a common "missed variant" and ignoring thisprwould increase the success rate to ~60%</li>
 <li>Sequences whose haplogroup required C169185 often did not have it, but was requenctly annotated with the closely adjacent T16187d and 16188.1T variants </li>

</ol>

The C16189T variant in mitochondrial DNA has been identified as a challenging marker due to its high recurrence and potential for misidentification in automated haplogroup classification tools. Studies have reported heteroplasmy at this position, indicating the coexistence of multiple mitochondrial DNA variants within an individual. For instance, research has shown that the level of heteroplasmy of the C16189T variant remained stable over time in cervical cells, suggesting its persistence within individuals.
pmc.ncbi.nlm.nih.gov
Additionally, the C16189T variant has been associated with various multifactorial diseases, such as metabolic syndrome and endometrial cancer, highlighting its clinical significance.
researchgate.net
These findings underscore the importance of precise variant detection and interpretation in mitochondrial DNA studies, as misidentification can lead to erroneous haplogroup assignments and impact phylogenetic reconstructions.


| Variants Combination               | Count  |
|-------------------------------------|--------|
| T16187d                            | 8059   |
| T16187d, 16188.1T                   | 35486  |
| C16189T                            | 206    |
| T16187d, C16189T                    | 77     |
| 16188.1T                           | 94     |
| T16187d, C16189T, 16188.1T          | 5      |
| T16187d, 16188.1T, C16189T          | 1      |



<img src="https://github.com/waigitdas/Mitochondrial-DNA-Research/blob/main/Knowledge_Graph/images/C16189T_Veen_diagram.png" width="50%" height="50%">
