Psychosomatic Disease Knowledge Graph Analysis

This repository contains comprehensive datasets and analytical results from our research on psychosomatic disease relationships, presented in both Chinese and English to facilitate global collaboration.

📁 File Structure

• `Chinese/`: Original Chinese datasets

• `English/`: English translated versions


📊 File Descriptions

1. Co-Drugs.xlsx
| Column | Content                  |
|--------|--------------------------|
| 1      | Disease entity A         |
| 2      | Disease entity B         |
| 3      | Number of shared drugs   |
| 4      | Network distance between diseases |

---

2. Co-Symptoms.xlsx
| Column | Content                  |
|--------|--------------------------|
| 1      | Disease entity A         |
| 2      | Disease entity B         |
| 3      | Number of shared symptoms |
| 4      | Network distance between diseases |

---

3. Drugs_Semantic.xlsx
| Column | Content                  |
|--------|--------------------------|
| 1      | Disease entity A         |
| 2      | Disease entity B         |
| 3      | Semantic similarity score (0-1) |
| 4      | Network distance between diseases |

---

4. Relative_Risk.xlsx
| Column | Content                  |
|--------|--------------------------|
| 1      | Symptom entity A         |
| 2      | Symptom entity B         |
| 3      | Co-occurrence frequency  |
| 4      | Frequency of symptom A   |
| 5      | Frequency of symptom B   |
| 6      | Expected co-occurrence frequency |
| 7      | Relative risk score      |
| 8      | Network distance between symptoms |

---

5. Symptom_Lcc.xlsx
| Column | Content                  |
|--------|--------------------------|
| 1      | Symptom entity           |
| 2      | LCC size                 |
| 3      | Diameter d_s             |
| 4      | lcc [rand]               |
| 5      | z-score                  |

---

6. Symptom_Separation.xlsx
| Column | Content                  |
|--------|--------------------------|
| 1      | Disease entity A         |
| 2      | Disease entity B         |
| 3      | Network-diameter d_A     |
| 4      | Network-diameter d_B     |
| 5      | d_AB                     |
| 6      | S_ab                     |


7. Psychosomatic_Disease_Knowledge_Graph (RDF)
• Complete knowledge graph in RDF format

• Contains all entities and relationships referenced in the Excel files


🌐 Usage
• Chinese version: Use files in `Chinese/` folder

• English version: Use files in `English/` folder

• All columns maintain consistent meaning across language versions
