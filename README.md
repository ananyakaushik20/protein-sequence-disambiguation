# protein-sequence-disambiguation

### Protein Sequence Disambiguation and Functional Annotation Pipeline

# Overview:
Engineered a sophisticated bioinformatics pipeline to disambiguate protein sequences from two assemblies of the same organism and identify proteins with specific enzymatic activities. This project involved intricate sequence alignment, redundancy reduction, and functional annotation, ensuring comprehensive and efficient handling of large-scale protein data.

### Key Components:

# Sequence Alignment and Disambiguation:

- Objective: Accurately disambiguate protein sequences from two assemblies (assembly_1.prot.fa and assembly_2.prot.fa) through precise mapping and alignment.
- Method: Implemented advanced pairwise local sequence alignment using the Smith-Waterman algorithm via Biopython’s PairwiseAligner.
- Scoring: Utilized the BLOSUM62 substitution matrix for optimal alignment scoring.
- Criteria: Defined stringent criteria with 95% sequence identity and 90% query coverage to ensure high accuracy.
- Output: Produced a consolidated FASTA file containing non-redundant protein sequences with both query and reference IDs included.


# Functional Annotation:

- Objective: Map standardized gene identifiers from assembly_2.prot.fa to UniProt identifiers and identify hydrolase proteins acting on ester bonds.
- Method: Extracted gene names from the reference assembly and interfaced with the UniProt REST API to obtain detailed protein annotations.
- Data Handling: Leveraged pandas for robust data manipulation and filtering.
- Output: Created comprehensive TSV files containing UniProt annotations and identified hydrolase proteins.


# Requirements:
- Programming Language: Python
- Libraries: Biopython, pandas
- Algorithms: Smith-Waterman for local sequence alignment, BLOSUM62 substitution matrix
- APIs: UniProt REST API

# Scalability and Robustness:

- Memory Management: Ensured efficient handling of large datasets using pandas and streaming data retrieval from APIs.
- Parallel Processing: Designed for potential integration of parallel sequence alignment to significantly enhance processing speed.
- Data Governance: Implemented thorough metadata logging and pipeline versioning to guarantee reproducibility and traceability of all analyses.
- Future-Proofing: Considered scalability for handling millions of proteins by optimizing memory usage and processing efficiency.

# Impact:
This pipeline exemplifies advanced bioinformatics capabilities, seamlessly integrating sequence alignment and functional annotation to facilitate large-scale protein analysis. The robust design ensures accuracy, efficiency, and scalability, making it a valuable tool for genomic research and biotechnological applications.
