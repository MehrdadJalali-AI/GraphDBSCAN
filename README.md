# GraphDBSCAN

<p align="center">
  <img src="GraphDBScan.png" alt="GraphDBScan" width="400" height="400">
</p>


# **Effect of Noise Removal on Graph Structure and Community Detection with Auto-encoder**

## **1. Graph Reduction & Noise Removal Impact**

| **Metric** | **Before Noise Removal** | **After Noise Removal** | **Change (%)** |
|------------|---------------------|------------------|------------------|
| **Nodes** | 1000 | 357 | 🔻 **-64.3%** (Noise removed) |
| **Edges** | 3503 | 811 | 🔻 **-76.8%** (Sparse edges removed) |
| **Density** | 0.0070 | 0.0114 | 🔺 **+62.9%** (Graph more connected) |

### **Analysis:**
- **643 nodes were removed**, indicating that a large portion of the original graph was noise.
- **Edges reduced by 76.8%**, showing that many weakly connected edges were eliminated.
- **Density increased by 62.9%**, proving that the remaining graph is **more structured and connected**.

✅ **Noise removal effectively removed weakly connected nodes, preserving a denser and more meaningful network.**

---

## **2. Impact on Node-Level Properties**

| **Metric** | **Before Noise Removal** | **After Noise Removal** | **Change (%)** |
|------------|---------------------|------------------|------------------|
| **Avg Degree** | 7.0060 | 4.5440 | 🔻 **-35.1%** (Fewer but stronger connections) |
| **Modularity** | 0.1025 | 0.4449 | 🔺 **+334.2%** (Stronger community structure) |
| **Clustering Coefficient** | 0.6309 | 0.4646 | 🔻 **-26.3%** (Fewer local clusters) |
| **Largest Connected Component Size** | 1000 | 291 | 🔻 **-70.9%** (Smaller core structure) |
| **Avg Shortest Path Length** | 4.0136 | 4.1683 | 🔺 **+3.9%** (Slightly longer paths due to noise removal) |

### **Analysis:**
- **Average Degree dropped (-35.1%)**, meaning nodes now maintain fewer but **more essential** connections.
- **Modularity increased (+334.2%)**, highlighting that **community detection significantly improved**.
- **Clustering Coefficient decreased (-26.3%)**, indicating that local clusters became less redundant.
- **Largest Connected Component (LCC) size reduced (-70.9%)**, confirming that **only the strongest core remains**.
- **Shortest Path Length increased (+3.9%)**, showing that nodes are now **more spread out but still connected**.

✅ **The graph is now more structured, with clearer community boundaries and reduced noise.**

---

## **3. Final Conclusion**

| **Observation** | **Effect of Noise Removal** |
|-----------------|---------------------------|
| 🔹 **Graph is smaller** | Reduced from **1000 → 357 nodes**, eliminating **64.3% noise**. |
| 🔹 **More meaningful edges** | Retained **core connectivity** with stronger structural integrity. |
| 🔹 **Community structure vastly improved** | **Modularity increased from 0.1025 → 0.4449**. |
| 🔹 **Graph properties changed significantly** | Increased **density**, improved **node importance**, and enhanced **community detection**. |

✅ **Noise removal effectively improved community structure, connectivity, and modularity, ensuring a cleaner and more structured network.**

---

