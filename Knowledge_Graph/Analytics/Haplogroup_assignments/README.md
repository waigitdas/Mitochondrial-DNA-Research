# Haplogroip Assignments
 
Haplogroup assignments were provided by the Mitomap team at Children's Hosdpital of Philadelphia. The used the Haplogrep3 tools. The assignments were added as a propterty to the Genbank sequence nodes. 

This project intended to replicate these assignmentsusing graph methods. That effort failed. The Excel workbooks in this folder Used traversals of the dnode (haplotree) paths from Eve to the assigned haplogroup node. show:

<ol>
 <li>Traversals to the assiggned hapolgroup node were successful foe only 34% of the Genbank sequences.</li>
 <li>The C16189T was a common "missed variant" and ignoring thisprwould increase the success rate to ~60%</li>
 <li>Sequences whose haplogroup required C169185 often did not have it, but was requenctly annotated with the closely adjacent T16187d and 16188.1T variants </li>

</ol>
The C16189T variant has long been recognized as a problematic marker in mitochondrial DNA studies due to its high recurrence and frequent misidentification in automated haplogroup classification tools. In the knowledge graph analysis, discrepancies in Haplogrep3’s variant calls flagged this issue, as the tool identified C16189T where the raw sequence data instead revealed a combination of T16187d and 16188.1T. This suggests that the widely accepted presence of C16189T in haplogroup definitions may be, at least in some cases, an artifact of alignment errors rather than a true defining mutation. The implications extend beyond this single variant—if a fundamental marker can be repeatedly misclassified, it raises broader concerns about the reliability of haplogroup assignments and the validity of the haplotree itself. Rather than an isolated error, this case serves as further evidence that the haplotree and its underlying classification tools are built upon assumptions that do not always hold up under closer scrutiny.

.


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

The case study of the 6 sequences with 3 variants in the 16189 region shows sequence which have C16189T and two closely adjacent variants. These complex matching challenges were handled correctly by the knowledge graph analytics. 
