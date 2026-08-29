# Computational Protein Engineering — O₂ Tunnel Analysis in Hydroxylases

Undergraduate research project investigating oxygen (O₂) transport 
tunnels in hydroxylase proteins using computational tools and 
ML-based approaches, with applications in biocatalysis.

## Research context

- **Institution:** IIT Mandi, BS Chemical Sciences (2024–2028) Minor Management
- **Supervisor:** Prof. Bhaskar Mondal, School of Chemical Sciences
- **Focus:** Predicting, engineering, and controlling O₂ transport 
  tunnels in hydroxylase proteins for biocatalytic applications
- **Status:** Active — ongoing (August 2026)

## Research direction

Hydroxylase enzymes catalyse the insertion of oxygen into substrate 
molecules — a critical reaction in biocatalysis. For this to occur, 
O₂ must travel from the protein surface to the buried active site 
through a physical tunnel. The geometry of this tunnel (length, 
bottleneck radius, hydrophobicity, lining residue composition) 
directly controls enzyme efficiency.

This project focuses on:
- Computational analysis of O₂ transport tunnels in hydroxylase proteins
- Feature extraction from tunnel geometry using CAVER and MDAnalysis
- ML-based prediction of tunnel properties (→ ProTunnelML)
- Engineering insights for improving biocatalytic activity

## Repository structure
/papers/ # Reading notes on key literature
/analysis/ # CAVER and MDAnalysis scripts
/data/ # Tunnel geometry datasets
/models/ # ML models for tunnel prediction (ProTunnelML)
/slides/ # Research discussion slides for Prof. Mondal
/notebooks/ # Exploratory analysis notebooks

## Tools and stack

Python · CAVER · MDAnalysis · ColabFold · PyMOL · BioPython · 
Scikit-learn · HuggingFace

## Related project

**ProTunnelML** — ML-enhanced protein tunnel prediction web app  
Built directly on data generated from this research.  
→ github.com/soham-bhandare-0406/ProTunnelML

## Contact

Soham Prakash Bhandare
BS Chemical Sciences, IIT Mandi  
B24004@students.iitmandi.ac.in
