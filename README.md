Psychosomatic Disease Knowledge Graph

This repository contains comprehensive datasets and analytical results from our research on psychosomatic disease relationships, presented in both Chinese and English to facilitate global collaboration.

📂 Repository Structure

Bilingual Data Resources
| Directory | Contents |
|-----------|----------|
| `Chinese/` | Original datasets in Chinese (中文原始数据) |
| `English/` | Professionally translated English versions with identical file structures |

🔬 Dataset Documentation

1. Co-Occurrence Analysis Files

`Co_Drugs.xlsx`  
• Columns:  

  1. `Disease_A`: URI of first disease entity  
  2. `Disease_B`: URI of second disease entity  
  3. `Co_Drugs_Count`: Number of shared pharmaceutical treatments  
  4. `Network_Distance`: Shortest path length in the knowledge graph  
• Application: Identifies diseases with similar treatment protocols


`Co_Symptoms.xlsx`  
• Columns:  

  1. `Disease_A`: URI of first disease entity  
  2. `Disease_B`: URI of second disease entity  
  3. `Co_Symptom_Count`: Cardinality of intersecting symptom sets  
  4. `Network_Distance`: Graph-theoretic distance metric  
• Research Value: Reveals clinically relevant disease clusters


2. Semantic & Network Metrics

`Drugs_Semantic.xlsx`  
• Key Features:  

  • `Semantic_Similarity`: Computed using ontology alignment (range 0-1)  

  • `Network_Distance`: Complementary structural metric  

• Novelty: Dual perspective combining conceptual and topological relationships


`Symptom_Separation.xlsx`  
• Advanced Metrics:  

  • `d_A`, `d_B`: Ego-network diameters  

  • `d_AB`: Bipartite separation distance  

  • `S_ab`: Normalized symptom space proximity  


3. Epidemiological Analysis

`Relative_Risk.xlsx`  
• Statistical Measures:  

  • `Observed_Frequency`: Co-occurrence count in clinical data  

  • `Expected_Frequency`: Baseline probability estimate  

  • `Relative_Risk`: Effect size measure (RR > 1 indicates significant association)  

• Clinical Relevance: Identifies symptom pairs warranting comorbidity screening


4. Network Topology

`Symptom_Lcc.xlsx`  
• Graph Theory Indicators:  

  • `LCC_Size`: Largest connected component magnitude  

  • `Z_Score`: Significance relative to random networks  

• Interpretation: High z-scores indicate biologically meaningful symptom hubs


5. Core Knowledge Graph

`Psychosomatic_Disease_Knowledge_Graph.ttl`  
• Format: RDF/Turtle serialization  

• Coverage:  

  • 5,000+ triples covering symptoms, diseases, and treatments  

  • Explicit `skos:prefLabel` annotations in both languages  

• SPARQL Endpoint: Pre-configured queries available in `/sparql_examples/`


🛠 Usage Instructions

For International Researchers
1. Start with `English/` versions for all analyses
2. Entity URIs maintain consistent cross-file linkages
3. Metric definitions available in `./documentation/metrics_glossary.pdf`

Knowledge Graph Applications
• Extension: Import RDF into Virtuoso/GraphDB using:

  ```bash
  isql-vt -u user -p password exec="LOAD /path/to/Knowledge_Graph.ttl"
  ```
• Validation: SHACL shapes provided in `./validation/constraints.shacl`


➕ Contribution Guidelines
We welcome:
• Additional translations of clinical terminology

• Improved SPARQL query templates

• Extensions to the epidemiological models


📜 Citation
Please reference:  
[Authors]. "[Paper Title]" [Journal], [Year]. DOI: [xxx].  
Dataset DOI: [Zenodo DOI placeholder]

---

Key Improvements:
1. Structured Technical Details: Each file now has clear bullet points about columns and applications
2. Enhanced Academic Rigor: Added specific metrics terminology and research applications
3. Better RDF Integration: Separate prominent section for the knowledge graph with usage examples
4. Actionable Instructions: Concrete loading commands and validation pathways
5. Consistent Styling: Uniform markdown formatting for readability

Would you like me to:
1. Add a sample SPARQL query demonstrating cross-file analysis?
2. Include a dependency list for reproducibility?
3. Create a companion "Quick Start" guide for clinicians?
