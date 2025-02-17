
# Missing Variants   
<h3><strong><em>Only 3% of sequences have all their haplogroup's defining variants!</em></strong></h3>

The knowledge graph contains a **list of variants** for each GenBank sequence and **two lists for each dnode tree branch**:  
1. **Branch-defining variants** – specific to the branch.  
2. **Path variants** – those that accumulate along the traversal from Eve to the branch.  

In the knowledge graph, **lists represent sets**, which can be analyzed using **set algebra**.  

## Set Algebra in Neo4j  
Neo4j's `apoc.coll.*` functions efficiently manage set operations, including:  

- **Subtraction (−):** `apoc.coll.subtract(A, B)`  
- **Intersection (∩):** `apoc.coll.intersection(A, B)`  
- **Containment (⊆):** `apoc.coll.containsAll(A, B)`  
- **Union (∪):** `apoc.coll.union(A, B)`  
- **Disjointness (∅):** `apoc.coll.disjoint(A, B)`  
- **Distinct extraction (∪ᵢ):** `apoc.coll.toSet(A)`  
- **List flattening (⋃):** `apoc.coll.flatten(A)`  
- **Duplicate neighbor removal (≡):** `apoc.coll.dropDuplicateNeighbors(A)`  
- **Sorting (⇑):** `apoc.coll.sort(A)`  

## Detecting Missing Variants  
Missing variants are identified by subtracting the **sequence variants** from the **path variants**:  

```cypher
apoc.coll.subtract(path_variants, sequence_variants)
```

## Key Observations from the Excel Workbook  
- **Only 3%** of GenBank sequences contain all the defining variants required for their assigned haplogroup.  
- **At least one sequence** in **99% of haplogroups** is missing required variants.  
- **Traversal failures:** All paths from Eve to a haplogroup node fail at some point due to missing variants.  
- **C16189T is the most commonly missed variant**, discussed in detail [here].  
- **"Missing" variant regions often contain mutations**—just not the ones expected to be there. See the discussion on **back mutations** [here].  

