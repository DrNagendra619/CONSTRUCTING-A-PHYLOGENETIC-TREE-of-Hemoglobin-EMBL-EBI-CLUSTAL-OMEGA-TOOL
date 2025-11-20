# CONSTRUCTING-A-PHYLOGENETIC-TREE-of-Hemoglobin-EMBL-EBI-CLUSTAL-OMEGA-TOOL
CONSTRUCTING A PHYLOGENETIC TREE of Hemoglobin EMBL-EBI CLUSTAL OMEGA TOOL
🩸 Hemoglobin Chain Phylogenetic Analysis (Clustal Omega)

This repository contains the input sequences, multiple sequence alignment (MSA), and phylogenetic analysis results for a set of known Hemoglobin protein chains, generated using the EMBL-EBI Clustal Omega tool. The goal is to determine the evolutionary relationships among these diverse α- and β-like Globin chains.

📁 Repository Contents

Filename,Description,Source
clustalo-I20250718-063254-0826-7058527-p1m.fa,Input FASTA File containing the 11 Hemoglobin chain sequences used for the analysis.,Input
Clustal Omega _ EMBL-EBI TOOL OUPUT.pdf,Summary of the Clustal Omega job execution and initial alignment output.,Output
Clustal Omega _ ALIGMENTS.pdf,Full Multiple Sequence Alignment (MSA) showing residue conservation (with color scheme).,Output
Clustal Omega _ EMBL-EBI PHYLOGENETIC TREE.pdf,Newick format of the Phylogenetic Tree (and its display).,Output
GUIDE TREE CLUSTAL OMEGA Hemoglobin PHYLOGRAM.png,Graphical representation of the Guide Tree (Phylogram).,Output
CLUSTAL OMEGA Hemoglobin RADIAL PHYLOGRAM.png,Graphical representation of the Phylogenetic Tree (Radial View).,Output
clustalo-I20250718-063254-0826-7058527-p1m-submission.xml,"XML file detailing the Clustal Omega execution parameters (e.g., seqtype: protein, outfmt: clustal_num).",Execution Details
🧬 Analysis Overview

1. Sequences and Alignment

The analysis included 11 Hemoglobin chains identified by their PDB IDs (e.g., 1HBR, 1A3N, 1GCW) and chain designator (1 or 2).

    Sequence Length: The sequences are around 135 to 146 residues long.

Highly Conserved Regions: The Multiple Sequence Alignment (MSA) shows significant conservation (indicated by * and : below the alignment) in key regions, particularly around the presumptive heme-binding pocket.

    The region near position 50 (in the α-chains) and the highly conserved histidine residues (e.g., the distal and proximal histidines, critical for oxygen binding) are well-aligned across most chains.

2. Phylogenetic Tree Results

The phylogenetic tree (constructed using the Neighbor-Joining method based on the MSA) clearly separates the sequences into two main clades, corresponding to the two major types of Hemoglobin chains:
Clade,Sequences (Examples),Branch Lengths (Similarity),Interpretation
Clade 1 (Alpha-like),"1HBR_1, 1A3N_1, 1HDA_1, 2D5X_1","Show very small branch lengths (e.g., 0.06025, 0.06028, 0.06029) within the group.","These sequences are highly conserved, likely representing Hemoglobin α chains from different species or slightly different human variants."
Clade 2 (Beta-like),"1HBR_2, 1A3N_2, 1HDA_2, 2D5X_2","Show larger branch lengths to the outgroups, but are closely grouped (e.g., 1A3N_2 and 1HDA_2 are very close).","These sequences are closely related, likely representing Hemoglobin β chains (or related chains like gamma/delta) from different species/variants."
Outgroups,"1VHB_1, 1GCW_1, 1GCW_2","Exhibit the longest branch lengths (1VHB_1: 0.50498, 1GCW_1: 0.33084, 1GCW_2: 0.34114).","These chains are the most divergent and represent more distantly related Globin proteins (e.g., non-mammalian, or Myoglobin/other Globin types)."
Key Finding: The distinct clustering confirms the long-established evolutionary divergence of the Hemoglobin α- and β-globin families.
ethods and Citation

Tool Used

    Program: Clustal Omega (version 1.2.4) 

Database: EMBL-EBI JDispatcher

Sequence Type: Protein

Output Format: Clustal with residue numbering (clustal_num).

How to Use This Data

The .fa and .clustal_num (in the PDF/text files) outputs can be used to re-run the analysis or be imported into visualization tools like MEGA or FigTree for custom tree rendering.

Citation

If you utilize this analysis in your work, please cite the Clustal Omega publication:

    Sievers F, et al. (2011). Fast, scalable generation of high-quality protein multiple sequence alignments using Clustal Omega. Molecular Systems Biology, 7(1): 539.
