# Philosophical Influence Network

This repository contains a Toy Example of code to visualize a small network of influences between historical philosophers. The project uses a simple, generated dataset to demonstrate how to map "influencer" to "influenced" connections and plot the resulting graph, serving as an introduction to network analysis.

## 📊 Data

The project uses a simplified internal dataset, which is generated within the notebook itself and saved as `influences_sample.csv`. Each row in this file represents a **directed influence connection**.

| Column | Description |
| :--- | :--- |
| `influencer` | The philosopher who exerted the influence. |
| `influenced` | The philosopher who received the influence. |
| `school` | Philosophical school or movement (e.g., `Ancient`, `Modern`, `German Idealism`). |
| `year_influencer` | Birth year of the influencing philosopher. |

**Philosophers in the Example:** The sample dataset includes notable figures such as Socrates, Plato, Aristotle, Immanuel Kant, Friedrich Nietzsche, and Martin Heidegger, among others.

## 💻 Methodology (`_network_plot.ipynb` Notebook)

The analysis follows three main steps to generate the visualization:

1.  **Data Loading and Preparation:** The influence data is loaded and structured using the `pandas` library.
2.  **Node and Edge Preparation:** A unique list of philosophers (the **nodes**) is created, and the influence connections (the **edges**) are mapped into index pairs. Initial node positions are randomly assigned in a 2D space for plotting.
3.  **Network Visualization:** The network is plotted using the `matplotlib` library. The visualization displays the nodes (blue circles) and the edges (gray lines) representing the direction of influence, under the title "Philosophical Influence Network — Toy Example".

## 🛠️ Requirements and Dependencies

To run the notebook and replicate the visualization, you will need the following Python libraries:

* `numpy`
* `pandas`
* `matplotlib`
* `os`

## 🚀 How to Run

1.  **Clone** this repository to your local machine.
2.  Open the `_network_plot.ipynb` file in a Jupyter environment (like JupyterLab or VS Code with a notebook extension) or Google Colab.
3.  **Run all cells** sequentially. The last cell will display the network visualization.
