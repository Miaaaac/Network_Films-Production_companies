# Analysis of Network Models for Film Co-Production Networks


This project compares three classical network models — **Erdős–Rényi (ER)**, **Watts–Strogatz (WS)**, and **Barabási–Albert (BA)** — with a real-world film co-production network.

The objective is to evaluate how well these standard models reproduce the structural characteristics observed in the real network and to identify the main strengths and limitations of each model.

The analysis focuses on three network measures:

- **Diameter**: the maximum shortest-path distance between any two nodes.
- **Average clustering coefficient**: the tendency of nodes to form tightly connected groups.
- **Average shortest path length**: the average number of edges required to connect pairs of nodes.

---

## Network Comparison

| Network | Diameter | Average Clustering | Average Shortest Path |
|---|---:|---:|---:|
| **Erdős–Rényi (ER)** | 3 | 0.010 (1%) | 2.59 |
| **Watts–Strogatz (WS)** | 23 | 0.371 (37%) | 11.38 |
| **Barabási–Albert (BA)** | 8 | 0.009 (0.9%) | 4.63 |
| **Real Co-Production Network** | 10 | 0.750 (75%) | 3.61 |

---

## Erdős–Rényi Model

The Erdős–Rényi model generates a network in which connections are created randomly. Each potential connection is formed independently according to a given probability. As a result, the model does not include an explicit mechanism for community formation or preferential attachment.

### Results

- **Diameter: 3**
- **Average clustering coefficient: 0.010 (1%)**
- **Average shortest path length: 2.59**

The diameter of 3 indicates that the network is highly compact. Even the most distant pair of companies can be connected through a very small number of intermediate nodes.

The average shortest path length of 2.59 further demonstrates the compactness of the network. On average, companies can reach one another through fewer than three connections.

However, the average clustering coefficient is only 0.01, or 1%. This indicates that triangles and tightly connected groups are very rare.

### Interpretation

The Erdős–Rényi model therefore captures the short-path characteristic of the real network, but it fails to reproduce its strong clustering and community structure.

Because connections are generated randomly, the model does not represent the repeated collaborations and tightly connected groups that characterize real film co-production networks.

Overall, the ER model produces a network that is compact but lacks meaningful structural organization.

---

## Watts–Strogatz Model

The Watts–Strogatz model was developed to reproduce small-world network characteristics. It combines local connectivity with random long-range connections, allowing the network to exhibit relatively high clustering while maintaining connections between distant parts of the network.

### Results

- **Diameter: 23**
- **Average clustering coefficient: 0.371 (37%)**
- **Average shortest path length: 11.38**

The Watts–Strogatz network has a substantially higher clustering coefficient than the Erdős–Rényi network. A value of 0.371 indicates that nodes are more likely to form interconnected local groups.

However, the diameter is 23, which is considerably larger than that of the real network. The average shortest path length is also high at 11.38, meaning that companies are, on average, separated by approximately 11 to 12 connections.

### Interpretation

The main strength of the Watts–Strogatz model is its ability to generate clustering. This makes it more representative of the local communities observed in real co-production networks than the Erdős–Rényi model.

However, the network is too dispersed compared with the empirical network. The real network has an average shortest path length of only 3.61, whereas the WS network has an average shortest path length of 11.38.

Therefore, although the Watts–Strogatz model captures aspects of clustering and small-world organization, it does not reproduce the combination of high clustering and short paths observed in the real network.

---

## Barabási–Albert Model

The Barabási–Albert model generates scale-free networks through preferential attachment. New nodes are more likely to connect to nodes that already have a high number of connections. This process results in the emergence of highly connected nodes, commonly referred to as hubs.

In the context of film production, these hubs can represent companies that participate in a large number of co-productions.

### Results

- **Diameter: 8**
- **Average clustering coefficient: 0.009 (0.9%)**
- **Average shortest path length: 4.63**

The diameter of 8 indicates that the network remains relatively compact. The presence of hubs helps reduce the maximum distance between nodes.

The average shortest path length is 4.63, which is relatively close to the value observed in the real network. Highly connected hubs provide efficient connections between different parts of the network.

However, the average clustering coefficient is only 0.009, or approximately 0.9%. This indicates that tightly interconnected groups are rare.

### Interpretation

The Barabási–Albert model successfully captures the presence of hubs, which is an important characteristic of the real film co-production network.

However, preferential attachment alone does not produce the high level of clustering observed in the empirical network. The real network has an average clustering coefficient of 75%, compared with only 0.9% in the BA model.

Therefore, the BA model captures network centralization and short paths relatively well, but it fails to reproduce the strong community structure present in the real network.

---

## Real Film Co-Production Network

The real film co-production network exhibits a combination of structural properties that are not simultaneously reproduced by any of the three standard models.

### Results

- **Diameter: 10**
- **Average clustering coefficient: 0.750 (75%)**
- **Average shortest path length: 3.61**

The clustering coefficient of 75% indicates a strong tendency for companies to form tightly interconnected groups. This suggests that companies frequently collaborate with other companies that are themselves connected, resulting in dense local communities.

At the same time, the average shortest path length of 3.61 indicates that the network remains highly accessible. Most companies can reach one another through only a small number of intermediate connections.

The network also contains highly connected companies that function as hubs. These hubs contribute to the overall connectivity of the network and help maintain short paths between different parts of the network.

The combination of high clustering, short paths, and hubs indicates that the empirical network has characteristics associated with both small-world and heterogeneous network structures.

---

## Analysis

The three standard models capture different aspects of the real co-production network.

### Erdős–Rényi

The Erdős–Rényi model produces very short paths and a compact network. However, its clustering coefficient is extremely low, meaning that it does not reproduce the strong communities observed in the real network.

### Watts–Strogatz

The Watts–Strogatz model produces substantially higher clustering than the ER model and therefore provides a better representation of local communities. However, its diameter and average shortest path are considerably larger than those of the real network.

### Barabási–Albert

The Barabási–Albert model produces highly connected hubs and relatively short paths. These characteristics are consistent with important features of the real network. Nevertheless, its clustering coefficient is extremely low, meaning that it fails to reproduce the dense collaborative communities observed in reality.

### Real Network

The empirical film co-production network combines all three important characteristics:

- **High clustering**
- **Short average path length**
- **Highly connected hubs**

This combination distinguishes the real network from the three standard theoretical models.

---


| Property | Erdős–Rényi | Watts–Strogatz | Barabási–Albert | Real Network |
|---|---|---|---|---|
| Short paths | Yes | No | Yes | Yes |
| High clustering | No | Moderate | No | Yes |
| Hubs | No specific mechanism | No specific mechanism | Yes | Yes |
| Strong community structure | No | Moderate | No | Yes |
| Overall representation | Limited | Partial | Partial | Empirical reference |

The results demonstrate that each theoretical model reproduces only certain characteristics of the empirical network.

- **Erdős–Rényi** captures random connectivity and very short paths.
- **Watts–Strogatz** captures clustering and aspects of small-world organization.
- **Barabási–Albert** captures preferential attachment, hubs, and relatively short paths.
- **The real network** combines high clustering, short paths, and hubs.

---

## Conclusion

The comparison demonstrates that none of the three standard network models fully reproduces the structural characteristics of the real film co-production network.

The Erdős–Rényi model produces a highly compact network but has almost no clustering. The Watts–Strogatz model generates substantially greater clustering but produces paths that are considerably longer than those observed in the empirical network. The Barabási–Albert model successfully produces hubs and relatively short paths but does not generate the high clustering required to represent the dense communities found in real co-production networks.

The real film co-production network is therefore characterized by the simultaneous presence of **high clustering, short average path lengths, and highly connected hubs**.

These results suggest that film-industry collaboration cannot be adequately represented by a single standard network-generation mechanism. A more realistic model would need to incorporate multiple mechanisms, potentially combining preferential attachment with community formation and repeated or localized collaboration.

The three classical models are therefore useful as theoretical benchmarks, but a model specifically designed to account for the structural characteristics of real film co-production networks would be required to provide a more accurate representation of the empirical system.
