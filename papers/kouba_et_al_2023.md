# Reading Notes — Kouba et al., ACS Catalysis 2023

**Full title:** Machine Learning-Guided Protein Engineering  
**Authors:** Petr Kouba, Pavel Kohout, Faraneh Haddadi, Anton Bushuiev,
Raman Samusevich, Jiri Sedlar, Jiri Damborsky, Tomas Pluskal,
Josef Sivic, Stanislav Mazurenko  
**Journal:** ACS Catalysis, 2023, 13(21), 13863–13895  
**DOI:** 10.1021/acscatal.3c02743  
**Type:** Perspective (review paper)  
**Read:** August 2026

---

## What this paper is

A comprehensive review of how machine learning is being applied
to protein engineering, written by researchers at Loschmidt
Laboratories (Masaryk University) and Czech Technical University.
It is a perspective paper — it surveys the field rather than
presenting original experimental results.

---

## Core argument

ML methods are increasingly central to biocatalyst engineering.
Rather than testing mutations one by one in the lab, ML can
leverage existing experimental and simulation data to predict
which mutations improve a target property — dramatically
accelerating the engineering cycle.

---

## What the paper covers (structure)

- **Section 2:** ML fundamentals and what makes protein data
  unique compared to other ML domains (sequences, structures,
  functional measurements, evolutionary information)

- **Section 3:** Comprehensive review of ML methods applied to
  protein engineering — spanning structure prediction, function
  annotation, stability, catalytic efficiency, enantioselectivity,
  solubility, and protein dynamics

- **Section 4:** Real-world case studies where ML was used to
  design improved enzymes and deploy them in practical
  biocatalysis applications

- **Section 5:** Current gaps and limitations — where ML still
  fails or produces unreliable predictions without experimental
  validation

- **Section 6:** What protein engineering can borrow from other
  ML-heavy fields to accelerate progress

---

## Key concepts introduced

**Supervised learning for proteins:**  
Train a model on labelled protein-property pairs
(sequence → stability, sequence → catalytic efficiency).
Requires experimental measurements as labels — expensive to
generate at scale.

**Self-supervised learning and protein language models:**  
Train on unlabelled protein sequences (the entire UniProt database)
by masking residues and predicting them. The model learns deep
evolutionary and structural representations without needing any
experimental labels. ESM-2 is the key example.

**Sequence-based vs structure-based approaches:**  
Sequence-based ML (protein language models) works from amino
acid sequences alone. Structure-based ML uses 3D atomic
coordinates from PDB structures. Both have tradeoffs —
sequences are abundant, structures are information-richer but
fewer in number.

**Fitness landscapes:**  
The mapping of all possible amino acid sequences to their
functional properties. ML tries to learn and navigate this
landscape to find high-fitness (high-activity) variants
without exhaustively testing every combination.

**Key warning from the authors:**  
Emerging ML models must be experimentally validated before
being trusted for rational protein design. High in silico
performance does not guarantee wet-lab success.

---

## Relevance to our O2 tunnel engineering project

This paper is the conceptual foundation for why ML is worth
applying to tunnel engineering in hydroxylases:

1. The same ML approaches reviewed here (structure-based
   prediction, fitness landscape navigation, stability
   prediction) are applicable to predicting tunnel properties
   (bottleneck radius, hydrophobicity, O2 transport efficiency)

2. The protein language model (ESM-2) discussed here is the
   exact model used in EnzyBERT (Project 2)

3. The authors' emphasis on experimental validation is a
   reminder that ProTunnelML predictions need to be grounded
   in real CAVER data from actual hydroxylase structures —
   not arbitrary inputs

4. Section 4 case studies show ML being used for enzyme
   engineering in industrial biocatalysis — directly the
   application domain Prof. Mondal is working in

---

## 3 questions for Prof. Mondal

1. The paper discusses ML for predicting stability and catalytic
   efficiency broadly — are there existing ML models specifically
   trained on tunnel geometry data, or is this an open gap we
   are filling with ProTunnelML?

2. The authors emphasise experimental validation of ML predictions.
   What wet-lab validation methods would be feasible for our
   tunnel predictions — mutagenesis studies, or MD simulations
   as a proxy?

3. The paper covers sequence-based and structure-based ML
   approaches. For tunnel engineering, should we focus on
   structure-based features from CAVER, or is there value in
   also incorporating sequence-level features from ESM-2?

---

## Citation (for future paper)

Kouba, P.; Kohout, P.; Haddadi, F.; Bushuiev, A.; Samusevich, R.;
Sedlar, J.; Damborsky, J.; Pluskal, T.; Sivic, J.; Mazurenko, S.
Machine Learning-Guided Protein Engineering.
*ACS Catal.* **2023**, *13* (21), 13863–13895.
https://doi.org/10.1021/acscatal.3c02743
