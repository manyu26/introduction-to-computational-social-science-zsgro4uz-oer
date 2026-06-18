## Getting started{{attrs[#blk-efv6ytcn2jqt]}}

Welcome to **Introduction to Computational Social Science**. This is your first study-guide section — replace it
with your own material. Each section keeps a permanent invisible label (the
`{{attrs[#…]}}` marker) so worksheets and slides generated from it stay
connected even as you edit.

Chemistry notation works out of the box: H~2~O, CO~3~^2-^, and equations like
$K_a = \frac{[\mathrm{H^+}][\mathrm{A^-}]}{[\mathrm{HA}]}$.

## What is Computational Social Science?{{attrs[#blk-gbkopfy2o7tp]}}

At its core, computational social science (CSS) is an interdisciplinary field that uses computational methods to analyze massive datasets about human behavior. Think of it as a powerful new toolkit for asking the classic questions of psychology—about thoughts, feelings, and actions—but at a scale and in contexts that were previously unimaginable.

Traditionally, a psychologist might study social anxiety by bringing 50 participants into a lab for a controlled interaction or by distributing a survey to a few hundred people. These methods are foundational and provide deep insights. CSS complements these approaches by leveraging the vast amount of digital data we create every day. This "digital exhaust"—our social media posts, search engine queries, GPS locations, online purchases, and even the text in our emails—provides a rich, if sometimes messy, record of human behavior in its natural environment.

Instead of a lab, the "field" for a computational social scientist might be Twitter. Instead of a survey, the "instrument" might be a computer program. Key methods in CSS include:

*   **Natural Language Processing (NLP):** Using algorithms to analyze text and speech. A psychologist could use NLP to scan millions of Reddit posts to measure changes in public sentiment about mental health or to identify linguistic markers that correlate with personality traits.
*   **Network Analysis:** Mapping and studying the relationships between people or entities. This is a natural fit for social psychology, allowing researchers to visualize how friendships form in a massive online community or how information (or misinformation) spreads through a social network.
*   **Agent-Based Modeling (ABM):** Creating computer simulations of social worlds. Researchers can program virtual "agents" with simple psychological rules (e.g., "avoid crowded spaces" or "interact with people similar to you") and observe what large-scale societal patterns emerge from these individual behaviors. This helps test theories about how micro-level psychology leads to macro-level phenomena.

The great promise of CSS is its ability to observe behavior at an unprecedented scale and with high **ecological validity**—that is, in the real-world settings where it naturally occurs. However, it also comes with significant challenges. The data is often unstructured and not collected with a specific research question in mind. More importantly, CSS raises critical ethical questions about privacy, consent, and algorithmic bias. Just because data is public doesn't mean it's ethical to use without consideration.

Ultimately, computational social science doesn't replace traditional psychological research; it enhances it. It offers a new lens through which to examine the human experience, allowing us to see patterns in the noise of our increasingly digital lives.

## Understanding Connections: An Introduction to Social Network Analysis{{attrs[#blk-agpfrsf47zv7]}}

Social Network Analysis (SNA) is a powerful method for studying social structures. Instead of focusing on individuals and their attributes (like age or income), SNA focuses on the *relationships and connections between them*. It allows us to visualize and measure the flow of information, influence, and interaction within a group. Think of it as creating a map of a social landscape.

### The Building Blocks of a Network

At its core, every network consists of two fundamental components:

*   **Nodes (or Vertices):** These are the individual actors or entities within the network. In a social network, nodes are typically people, but they could also be organizations, websites, or even countries.
*   **Edges (or Ties):** These are the connections or relationships between the nodes. An edge between two people could represent friendship, communication, collaboration, or a family tie.

Edges can have important properties:

*   **Undirected vs. Directed:** An **undirected** edge represents a reciprocal, two-way relationship. For example, being friends on Facebook is usually mutual. If Alice is friends with Bob, Bob is friends with Alice. A **directed** edge represents a one-way relationship. On Twitter, Alice can follow Bob without Bob following Alice back. The direction of the connection matters.
*   **Weighted:** Edges can also have **weights** to represent the strength or intensity of a connection. For example, an edge between two people could be weighted by the number of emails they exchanged in a month.

### Measuring Importance: Key Network Metrics

Once we have a network, we can analyze its structure using various metrics. Centrality measures are among the most common, helping us identify the most "important" or "influential" nodes in a network.

*   **Degree Centrality:** This is the simplest measure. A node's degree is simply the number of edges connected to it. In a social network, it represents a person's number of direct connections or friends. It's a rough measure of popularity. For directed networks, we can distinguish between *in-degree* (number of incoming connections, like followers) and *out-degree* (number of outgoing connections, like accounts followed).
*   **Betweenness Centrality:** This metric identifies "bridges" or "brokers" in a network. It measures how often a node lies on the shortest path between two other nodes. A node with high betweenness centrality has significant influence over the flow of information in the network and can act as a critical link connecting different clusters or groups.
*   **Closeness Centrality:** This measures how close a node is to all other nodes in the network. It's calculated as the average length of the shortest path from that node to every other node. A node with high closeness centrality can spread information very efficiently to the entire network.

### A Practical Example in Python

Let's build and analyze a small network using Python's popular `networkx` library. This code creates a simple, undirected network of friends and calculates their centrality scores.

```python
import networkx as nx
import matplotlib.pyplot as plt

# 1. Create a new, empty graph
G = nx.Graph()

# 2. Add nodes (the people in our network)
nodes_to_add = ["Alice", "Bob", "Charlie", "Diane", "Eve"]
G.add_nodes_from(nodes_to_add)

# 3. Add edges (the friendships)
edges_to_add = [("Alice", "Bob"), ("Alice", "Diane"), ("Bob", "Charlie"),
                ("Bob", "Diane"), ("Charlie", "Diane"), ("Diane", "Eve")]
G.add_edges_from(edges_to_add)

# 4. Calculate centrality measures
degree_centrality = nx.degree_centrality(G)
betweenness_centrality = nx.betweenness_centrality(G)
closeness_centrality = nx.closeness_centrality(G)

# Print the results for one person, Diane
print(f"Diane's Degree Centrality: {degree_centrality['Diane']:.2f}")
print(f"Diane's Betweenness Centrality: {betweenness_centrality['Diane']:.2f}")
print(f"Diane's Closeness Centrality: {closeness_centrality['Diane']:.2f}")

# 5. Visualize the network
nx.draw(G, with_labels=True, node_color='skyblue', node_size=2000, font_size=12)
plt.show()
```

When you run this code, you'll see that Diane has the highest scores for all three centrality measures.
*   **Degree:** She is connected to 4 out of 4 other people, making her the most directly connected.
*   **Betweenness:** She acts as the primary bridge. For Charlie to connect to Alice or Eve, the shortest path goes through Diane.
*   **Closeness:** Because she is so central, she can reach everyone else in the network more quickly (in fewer "hops") than anyone else.

This simple example shows how SNA can turn a list of connections into a rich, quantitative understanding of social structure and influence.

## What is Computational Social Science?{{attrs[#blk-mc1y5m2b857l]}}

Computational Social Science (CSS) is an interdisciplinary field that uses computational methods to analyze and understand human social behavior. It combines theories and questions from the social sciences (like sociology, political science, and economics) with techniques from computer science and data science. By analyzing large-scale datasets, running simulations, and building models, researchers in CSS aim to uncover patterns and dynamics of social life that were previously difficult or impossible to study.

## Key Concepts in Social Networks: Ego and Alter{{attrs[#blk-my3qetsalaxh]}}

In the study of social networks, two fundamental terms are used to describe the individuals within a network from a specific viewpoint: ego and alter.

The **ego** is the central individual or node that is the focus of the analysis. When mapping a personal network, the ego is the "self" or the person from whose perspective the network is being viewed.

An **alter** is any other individual directly connected to the ego. The alters are the "others" in the ego's social environment. For example, if we were analyzing your network of friends, you would be the ego, and each of your friends would be an alter.
