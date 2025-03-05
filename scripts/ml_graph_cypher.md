MATCH (g:Gene) return properties(g) limit 1
MATCH (n) return labels(n) as node_labels, count(n) as counts
MATCH (n) remove n.embedding
MATCH (p:Phenotype) return keys(p) limit 1
