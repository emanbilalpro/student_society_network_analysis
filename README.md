# Student Society Network Analysis (2018–2019)

## Project Overview

This project examines the social network of students at Lahore University of Management Sciences (LUMS), Pakistan, based on their participation in extracurricular societies during the 2018–2019 academic year.

The analysis uses Python and Gephi to study the structure of the network, identify central students and societies, and examine overlapping society memberships.

## Dataset

The dataset contains 1,299 anonymized student records covering 11 extracurricular societies.

Each record contains a student ID and society memberships.

## Methodology

Three undirected networks are constructed:

1. Student Network: Two students are connected if they share at least one society. Edge weight represents the number of shared societies.

2. Society Network: Two societies are connected if they share students. Edge weight represents the number of shared students.

3. Bipartite Network: Students are connected directly to the societies in which they participate.

The following network measures are calculated:

- Degree and Weighted Degree
- Betweenness Centrality
- Closeness Centrality
- Eigenvector Centrality
- Diameter
- Connected Components
- Average Clustering Coefficient
- Average Shortest Path Length
- Society Membership Sizes and Overlaps

Student shortest-path measures use unweighted edges.
Society shortest-path measures use inverse-overlap distances, where stronger overlaps have shorter distances.

## Tools

- Python
- Pandas
- NumPy
- NetworkX
- Matplotlib
- Gephi
- Google Colab

## Project Structure

- student_society_analysis.ipynb: Analysis notebook
- README.md: Project overview and instructions
- RESULTS.md: Calculated network findings
- requirements.txt: Python dependencies
- data/: Original anonymized dataset
- paper/: Research paper
- outputs/: Statistics, graphs, and Gephi files

## Running the Analysis

1. Open student_society_analysis.ipynb in Google Colab
2. Run the cells in order
3. Upload the Excel dataset when prompted
4. Review the network statistics and visualizations
5. Download the results and Gephi files

## Network Visualization in Gephi

The outputs/gephi/ folder contains GEXF and CSV files for the student, society, and bipartite networks.

Open the GEXF files in Gephi to visualize the networks.

Layout algorithms such as ForceAtlas2 can be applied to examine network structure.

Node size and color can represent centrality, society membership, and other network attributes.

## Results

The calculated findings are documented in RESULTS.md.

All network measurements are calculated directly from the provided dataset.
