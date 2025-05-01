# Psychosomatic_Disease_Knowledge_Graph_Analysis
This repository contains datasets and results from our research focusing on Psychosomatic Disease Knowledge Graph.

This repository contains analytical outputs from our mental health knowledge graph study, with full bilingual support for global accessibility.

📁 File Structure

Bilingual Datasets
| Folder       | Contents |
|--------------|----------|
| `Chinese/`   | Original datasets in Chinese |
| `English/`   | Complete English translations with identical file structure |

🔍 Dataset Descriptions

1. Co-Occurrence Analysis
| File | Columns | Description |
|------|---------|-------------|
| `Co_Drugs.xlsx` | 1-2: Disease entities<br>3: Co-prescribed drugs count<br>4: Network Distance | Measures therapeutic overlap between disease pairs |
| `Co_Symptoms.xlsx` | 1-2: Disease entities<br>3: Shared symptom count<br>4: Network Distance | Quantifies clinical presentation similarity |

2. Semantic & Topological Metrics
| File | Key Metrics |
|------|-------------|
| `Drugs_Semantic.xlsx` | 1-2: Disease entities<br>3: Semantic similarity (0-1 scale)<br>4: Network Distance | Combines ontological and structural relationships |
| `Symptom_Separation.xlsx` | 1-2: Disease entities<br>3-4: Network diameters (d_A, d_B)<br>5: d_AB<br>6: S<sub>ab</sub> | Calculates disease pair separation in symptom space |

3. Epidemiological Measures
| File | Advanced Metrics |
|------|------------------|
| `Relative_Risk.xlsx` | 1-2: Symptom entities<br>3: Co-occurrence frequency<br>4-5: Individual frequencies<br>6: Expected frequency<br>7: Relative Risk<br>8: Network Distance | Identifies statistically significant symptom clusters |

4. Network Topology
| File | Graph Theory Measures |
|------|-----------------------|
| `Symptom_Lcc.xlsx` | 1: Symptom entity<br>2: LCC size<br>3: Diameter (d<sub>s</sub>)<br>4: lcc[rand]<br>5: z-score | Quantifies symptom centrality in the knowledge graph |

5.Psychosomatic_Disease_Knowledge_Graph RDF

🛠 Usage Guide

For Non-Chinese Researchers
1. Use the `English/` versions of all files
2. Column headers follow this convention:
   • `[Entity1]`, `[Entity2]`: Always refer to medical concepts

   • `[Metric]_[unit]`: All calculated values are explicitly labeled

Knowledge Graph Construction
These analytical outputs can:
• Enhance existing KGs by importing the `*.rdf` files into Neo4j or RDF triplestores
