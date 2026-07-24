# 🧬 NGS Data Logistics

## 📖 Project Overview

This tutorial demonstrates a complete **Next-Generation Sequencing (NGS)** analysis workflow using **Galaxy**. The objective is to process raw sequencing data, identify genetic variants, and determine whether *Plasmodium falciparum* samples carry mutations associated with **Pyrimethamine resistance**.

The tutorial follows a realistic research scenario using publicly available sequencing datasets from the **MalariaGEN** project.

---

# 🦟 Background

Malaria is a life-threatening infectious disease caused by **_Plasmodium_** parasites and transmitted through the bites of infected female **_Anopheles_** mosquitoes.

One commonly used antimalarial drug is **Pyrimethamine**. However, resistance to this drug can occur due to mutations in the **_dhfr_** gene (**PF3D7_0417200**) of *Plasmodium falciparum* (Cowman *et al.*, 1988).

In this tutorial, sequencing data from **four infected individuals** is analyzed to determine which samples contain mutations associated with **Pyrimethamine resistance**.

---

# 🎯 Objective

Using paired-end sequencing data, the workflow aims to:

- 📥 Import raw FASTQ datasets
- 📂 Organize sequencing files into collections
- 🧬 Align sequencing reads to the *P. falciparum* reference genome
- 📊 Perform variant calling
- 📑 Convert variant data into tabular format
- 🔍 Identify samples carrying drug-resistance mutations

---

# 🔄 Workflow Overview

The complete analysis pipeline is illustrated below.

<p align="center">
  <img src="./collection_lifecycle.svg" alt="NGS Collection Lifecycle" width="100%">
</p>

<p align="center">
<i><b>Figure 1.</b> Overview of the NGS analysis workflow.</i>
</p>

### Workflow Summary

```text
FASTQ Files
      │
      ▼
Dataset Collection
      │
      ▼
Read Mapping
      │
      ▼
BAM Files
      │
      ▼
Variant Calling
      │
      ▼
VCF Files
      │
      ▼
Tabular Conversion
      │
      ▼
Merged Variant Dataset
      │
      ▼
Identification of Drug-Resistance Mutations
```

---

# 🧬 From Reads to Variants

The analysis uses paired-end sequencing datasets generated through the **MalariaGEN** initiative.

Each biological sample consists of:

- 🔴 Forward Reads (R1)
- 🔵 Reverse Reads (R2)

These paired-end reads are processed together throughout the workflow to improve alignment accuracy and variant detection.

---

# 📂 Sequencing Samples

| Sample Accession | Collection Site |
|-----------------|-----------------|
| **ERR636434** | Ivory Coast |
| **ERR636028** | Ivory Coast |
| **ERR042232** | Colombia |
| **ERR042228** | Colombia |

These sequencing datasets are publicly available through the **NCBI Sequence Read Archive (SRA)**.

---

# 🛠️ Bioinformatics Workflow

The Galaxy workflow includes the following major steps:

1. Import sequencing datasets
2. Create dataset collections
3. Quality assessment of sequencing reads
4. Align reads to the *P. falciparum* reference genome
5. Generate BAM alignment files
6. Perform variant calling
7. Produce VCF files
8. Convert variants to tabular format
9. Merge results for comparative analysis
10. Identify mutations associated with Pyrimethamine resistance

---

# 🎓 Learning Outcomes

By completing this tutorial, I learned how to:

- Work with paired-end NGS datasets
- Manage dataset collections in Galaxy
- Perform reference-based genome alignment
- Generate and interpret BAM and VCF files
- Detect genomic variants associated with drug resistance
- Apply an end-to-end variant analysis workflow using Galaxy
