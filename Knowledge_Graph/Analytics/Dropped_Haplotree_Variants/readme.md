# Dropped Variants
<h3><strong><em>Only 1% of sequences inherit all variants from haplogroup parent sequences</em></strong></h3>


This folder has files evaluating missing variants from the perspective of parent-child haplogroups in the haplotree. Sequences have assigned haplogroups. This assignment was done using the variant lists for the sequence. The dnode tree is derived from the haplotree, with back mutations removed. Each sequence is linkedto the haplotree by a seq_dnode relationship. The haplotree hierarchy is rendered with the dnode_child relationship. We can then create a hg_parent_child relationship which links together sequences which have haplogroups that are in a parent-child relationship in the haplotree. 

<img src="https://github.com/waigitdas/Mitochondrial-DNA-Research/blob/main/Knowledge_Graph/images/hg_parent_child_example.png" width="50%" height="50%">

We can now compare the parent and child sequences using set algebra. By subtracting  the child path variants from  the parent path variants we see any variants that were dropped ... that is, not passed down as would be expected. There are 2,215,069 possibe hg_parent_child relationship. The comparison reveals 2,190,125 sequence pairs with dropped variants. Thus, only 1.12% of sequence pair have the expected outcome. The dropped variants are detailed in the Excel in this folder.

<!--The hg_parent_child property of dropped_path_variants has this for the illustratedexample. [T63C,G66A,C152T,C195T,T6185C,A6575G,A12850G,T16381C].  We would expect the child sequence 	MG272956 to shared all path variantswith MG272663, but 8 variants are dropped.

The dropped variants reported exclude any back mutations appearing in the parent node.  The term dropped distinguishes them from back mutations. The term dropped is also distinct from "missing" because dropped has a context that missed lacks. 
-->
