# 📧 Email Network Analysis using NetworkX

This project explores the structure and connectivity of a company's internal email communication network using graph analysis with Python's NetworkX library.

Each node represents an employee, and each directed edge represents an email sent from one employee to another. The analysis answers key structural questions about the network, such as connectivity, component sizes, communication paths, and clustering properties.

## 📂 Dataset

The dataset is stored in `data/email_network.txt`, where:
- Each line represents an email with format: `sender<TAB>recipient<TAB>timestamp`
- The direction of the edge implies the direction of communication.

## 🧠 Project Objectives

- Load and process a directed multigraph from the dataset
- Determine strong and weak connectivity across the network
- Extract the largest strongly connected component (G_sc)
- Analyze key network metrics such as:
  - Average shortest path length
  - Graph diameter and radius
  - Periphery and center nodes
  - Shortest paths matching diameter
- Simulate information disruption scenarios by identifying key nodes
- Convert to undirected graph and measure transitivity and clustering

## ⚙️ Technologies Used

- Python 3
- NetworkX
- Jupyter Notebook or Python Script

## 📊 Key Results

- **Total Employees (Nodes)**: 167
- **Total Email Edges**: 82,927
- **Largest Strongly Connected Component**: 126 nodes
- **Diameter of G_sc**: 3
- **Average Shortest Path in G_sc**: ≈ 1.65
- **Transitivity of Undirected Graph**: ≈ 0.57
- **Average Clustering Coefficient**: ≈ 0.70

## 📁 File Structure

```
email-network-analysis/
├── data/
│   └── email_network.txt        # Raw dataset
├── network_connectivity_analysis.py  # Python script with answers to all 14 questions
├── README.md                    # Project overview and description
├── LICENSE                      # MIT License
└── .gitignore                   # Python environment ignores
```

## ✅ How to Run

1. Clone the repo or download the files
2. Install dependencies:
   ```bash
   pip install networkx
   ```
3. Run the Python file:
   ```bash
   python network_connectivity_analysis.py
   ```

## 👤 Author

- Mukesh Thenraj | [GitHub](https://github.com/Mukeshthenraj)

## 🪪 License

This project is licensed under the [MIT License](LICENSE).
