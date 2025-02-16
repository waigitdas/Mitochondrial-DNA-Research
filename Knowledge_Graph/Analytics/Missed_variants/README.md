# Missing Variants
 
The knowledge graph have List of variants for each Genbank sequence and two Lists for each dnode tree branch, one for the branch defining variants and the other forthe path variants which accrue during the traversal from Eve to the branch. List is a dattype in the knowledge graph that represent <b>sets</b> which can be analyzed using set algebra..

The Neo4j apoc.coll.* functions efficiently manage set algebra, including subtraction (−) with apoc.coll.subtract, intersection (∩) with apoc.coll.intersection, containment (⊆) with apoc.coll.containsAll, union (∪) with apoc.coll.union, disjointness (∅) with apoc.coll.disjoint, distinct element extraction (∪ᵢ) with apoc.coll.toSet, list flattening (⋃) with apoc.coll.flatten, duplicate neighbor removal (≡) with apoc.coll.dropDuplicateNeighbors, and sorting (⇑) with apoc.coll.sort, enabling flexible and optimized collection handling in Cypher queries.

Missing variants are detected by subtracting the sequence variants from the path_variants. In the Excel workbook in this folder, we see these facts:

<ol>
 <li></li>
 <li></li>
 <li></li>
 <li></li>
 <li></li>
 <li></li>
 <li></li>
</ol>
