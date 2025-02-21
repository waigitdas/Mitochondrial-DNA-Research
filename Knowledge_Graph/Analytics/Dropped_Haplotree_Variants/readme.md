# Dropped Variants

This folder has files evaluating missing variants from the perspective of parent-child haplogroups in the haplotree. Sequences have assigned haplogroups. This assignment was done using the variant lists for the sequence. The dnode tree is derived from the haplotree, with back mutations removed. Each sequence is linkedto the haplotree by a seq_dnode relationship. The haplotree hierarchy is rendered with the dnode_child relationship. We can then create a hg_parent_child relationship which links together sequences which have haplogroups that are in a parent-child relationship in the haplotree. 

<img src="https://github.com/waigitdas/Mitochondrial-DNA-Research/blob/main/Knowledge_Graph/images/hg_parent_child_example.png" width="50%" height="50%">
