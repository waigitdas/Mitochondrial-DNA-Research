# Mitochondrial DNA Knowledge Graph

 ### Key takeaways
<ol>
 <li>Probes aremuch more speficity than individual variants.</li>
 <li>Ony 3% of sequences have all the variants required for their haplogroup assignment</li>
 <li>Only 1% of sequences have the same number of path variants as sequences in their parent haplogroup</li>
 <li>Traversals for paths from Eve to nodes for the assigned haplogroup fail for lack of required variants</li>
 <li>The haplotree model is fatally flawed.</li>
</ol>

A mitochondrial DNA (mtDNA) knowledge graph (KG) was constructed in sequential steps in a Neo4j native graph database. GenBank full sequences were loaded into mt_seq nodes with their assigned haplogroup recorded as a property. The sequences were parsed using 40-base reference probes, producing in silico probes. Overlapping probes were stitched together and flanking regions from the full sequences added to ensure unique targeting to homologous positions in the reference sequence. The alignment of probes with the homologous reference sequence enabled comparisons using the diff-match-patch (DMP) algorithm, facilitating the annotation of probes with variants. Relationships between mt_seq, probe, and variant nodes formed the core of the initial graph.

The mtDNA haplotree was loaded into the KG and used to generate a derivative descendancy graph, which replicated the haplotree’s branching structure while harmonizing haplogroup naming and pruning variants that were absent from the full sequence data. The knowledge graph was enhanced by memorialized analytical results within the KG by ddition of new nodes, relationships, or properties.

A key finding was that most traversals from the haplotree root node (Eve) to the dnode representing the assigned haplogroup failed. These traversals depended on comparing the defining variants of each dnode to those observed in the test sequence, with failure indicating a lack of concordance. Identified causes included back mutations present in branch definitions but absent in the data, errors in variant annotation, and structural flaws in the haplotree model. While the model appears coherent at a high level, it breaks down when examined in granular detail where only 3% of sequences contain all required variants for their assigned haplogroup. 

