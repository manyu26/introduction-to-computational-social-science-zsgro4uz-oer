## Overview{{attrs[#blk-mc1y5m2b857l]}}

Computational Social Science (CSS) is an interdisciplinary field that uses computational methods to analyze and understand human social behavior. It combines theories and questions from the social sciences (like sociology, political science, and economics) with techniques from computer science and data science. By analyzing large-scale datasets, running simulations, and building models, researchers in CSS aim to uncover patterns and dynamics of social life that were previously difficult or impossible to study.

## What is Computational Social Science?{{attrs[#blk-gbkopfy2o7tp]}}

At its core, computational social science (CSS) is an interdisciplinary field that uses computational methods to analyze massive datasets about human behavior. Think of it as a powerful new toolkit for asking the classic questions of psychology—about thoughts, feelings, and actions—but at a scale and in contexts that were previously unimaginable.

Traditionally, a psychologist might study social anxiety by bringing 50 participants into a lab for a controlled interaction or by distributing a survey to a few hundred people. These methods are foundational and provide deep insights. CSS complements these approaches by leveraging the vast amount of digital data we create every day. This "digital exhaust"—our social media posts, search engine queries, GPS locations, online purchases, and even the text in our emails—provides a rich, if sometimes messy, record of human behavior in its natural environment.

Instead of a lab, the "field" for a computational social scientist might be Twitter. Instead of a survey, the "instrument" might be a computer program. Key methods in CSS include:

*   **Natural Language Processing (NLP):** Using algorithms to analyze text and speech. A psychologist could use NLP to scan millions of Reddit posts to measure changes in public sentiment about mental health or to identify linguistic markers that correlate with personality traits.
*   **Network Analysis:** Mapping and studying the relationships between people or entities. This is a natural fit for social psychology, allowing researchers to visualize how friendships form in a massive online community or how information (or misinformation) spreads through a social network.
*   **Agent-Based Modeling (ABM):** Creating computer simulations of social worlds. Researchers can program virtual "agents" with simple psychological rules (e.g., "avoid crowded spaces" or "interact with people similar to you") and observe what large-scale societal patterns emerge from these individual behaviors. This helps test theories about how micro-level psychology leads to macro-level phenomena.

The great promise of CSS is its ability to observe behavior at an unprecedented scale and with high **ecological validity**—that is, in the real-world settings where it naturally occurs. However, it also comes with significant challenges. The data is often unstructured and not collected with a specific research question in mind. More importantly, CSS raises critical ethical questions about privacy, consent, and algorithmic bias. Just because data is public doesn't mean it's ethical to use without consideration.

Ultimately, computational social science doesn't replace traditional psychological research; it enhances it. It offers a new lens through which to examine the human experience, allowing us to see patterns in the noise of our increasingly digital lives.

## Core Concepts and Methods{{attrs[#blk-9is6g3jjrhjl]}}

Computational social science is a diverse field that combines social theories with computational tools. This course will introduce you to the core methods and concepts used to analyze the digital traces of human behavior. Key topics include:

*   **Working with Digital Data:** We'll explore how to collect and manage the massive datasets that fuel computational social science. This includes data from social media platforms, digitized historical records, and information gathered by scraping websites. We'll also discuss the critical ethical considerations of privacy and consent when working with this "found" data.

*   **Social Network Analysis:** This method focuses on relationships and connections. By representing individuals or groups as **nodes** and their relationships as **edges**, we can map social structures, identify influential actors, and understand how information or behaviors spread through a population.

*   **Analyzing Text as Data:** With so much of modern communication happening through text, we need methods to analyze it at scale. Using techniques from Natural Language Processing (NLP), we can perform **sentiment analysis** to gauge public mood, use **topic modeling** to discover the main themes in thousands of documents, and study how language use varies across communities.

*   **Agent-Based Modeling (ABM):** How do large-scale social patterns emerge from individual behaviors? ABMs allow us to create simulations, or "artificial societies," where we program individual agents with simple rules and observe the collective outcomes. This is a powerful tool for testing social theories and exploring "what if" scenarios that are difficult to study in the real world.

*   **Machine Learning:** This involves using algorithms to learn patterns from data and make predictions. We'll cover **supervised learning**, where we train a model to predict a known outcome (e.g., classifying a news article as real or fake), and **unsupervised learning**, where we ask the algorithm to find hidden structures or groups within the data on its own.

Throughout all these topics, we will continuously engage with the **ethical dimensions** of computational research. Questions of algorithmic bias, data privacy, transparency, and the societal impact of our findings are central to practicing computational social science responsibly.

## Key Topics in Computational Social Science{{attrs[#blk-2178nqyurp6i]}}

Computational social science is an interdisciplinary field that draws on a diverse toolkit to study human behavior and social phenomena. An introductory course will typically focus on several core areas, each providing a unique lens for analysis.

*   **Digital Traces and Big Data:** This is the foundation for much of CSS. It involves collecting and analyzing the massive datasets generated by our digital activities. These "digital traces" can include everything from social media posts and search engine queries to mobile phone location data and online shopping records. A key challenge is learning how to ethically source, clean, and manage this data to answer social science questions.

*   **Network Analysis:** This topic focuses on the relationships and connections between entities (people, organizations, ideas, etc.). Social systems are viewed as networks of **nodes** (the entities) connected by **edges** (the relationships). Network analysis allows us to map these connections, identify influential actors, find hidden communities, and understand how information or diseases spread through a population.

*   **Text Analysis and Natural Language Processing (NLP):** A huge portion of digital data is unstructured text. Text analysis provides methods for extracting meaning from large volumes of text data. Techniques range from simple word counts and **sentiment analysis** (determining if a text is positive, negative, or neutral) to more advanced **topic modeling** (algorithmically discovering the main themes in a collection of documents).

*   **Agent-Based Modeling (ABM) and Simulation:** While other methods analyze existing data, simulation allows us to *generate* data to test social theories. In an agent-based model, a researcher creates a virtual environment populated by autonomous "agents" who follow a set of simple rules. By observing the large-scale, or **emergent**, patterns that arise from these local interactions, we can explore complex phenomena like traffic jams, market crashes, or the spread of opinions.

*   **Machine Learning for Social Inquiry:** Machine learning provides a set of powerful algorithms for finding patterns and making predictions from data. In social science, it can be used for tasks like:
    *   **Classification:** Predicting a categorical outcome, such as whether a person will vote or whether a piece of online content is misinformation.
    *   **Clustering:** Identifying natural groupings within a population based on their attributes, without pre-existing labels.
    *   **Prediction:** Forecasting future trends, such as unemployment rates or disease outbreaks, based on historical data.

*   **Ethics and Privacy:** A crucial and overarching theme is the ethical responsibility that comes with using large-scale human data. This includes topics like informed consent, data privacy and security, algorithmic bias, and the potential for misuse of research findings. A core principle in CSS is to balance the pursuit of knowledge with the protection of individuals and communities.

## Machine Learning in Social Science

Machine learning (ML) is a subfield of artificial intelligence that gives computers the ability to learn from data without being explicitly programmed. In computational social science, ML is a powerful tool for finding patterns, making predictions, and testing theories using large and complex datasets. Instead of a researcher defining a specific statistical model (e.g., linear regression with pre-selected variables), ML algorithms can often discover more complex, non-linear relationships within the data.

### Types of Machine Learning

*   **Supervised Learning:** This is the most common type of ML used in social science. The goal is to train a model to predict a known outcome or "label." The algorithm learns from a dataset where the correct answers are already provided (labeled data).
    *   **Classification:** The outcome is a category. For example, using the text of a social media post to classify it as hate speech or not hate speech.
    *   **Regression:** The outcome is a continuous value. For example, predicting a person's income based on their demographic data and online behavior.
    *   Common algorithms include logistic regression, support vector machines (SVMs), decision trees, and random forests.

*   **Unsupervised Learning:** In this case, the data is not labeled. The goal is for the algorithm to discover hidden structures or patterns on its own.
    *   **Clustering:** The algorithm groups similar data points together. A sociologist might use clustering to identify distinct communities within a social network based on communication patterns.
    *   **Dimensionality Reduction:** This simplifies complex datasets by reducing the number of variables while retaining important information. Principal Component Analysis (PCA) is a common technique.

*   **Reinforcement Learning:** While less common in CSS, this area of ML involves training "agents" to make a sequence of decisions in an environment to maximize a cumulative reward. It has potential applications in modeling social learning and strategic interaction.

### The ML Workflow and Key Considerations

A typical machine learning project involves several key steps and challenges:

*   **Feature Engineering:** This is the process of selecting and transforming raw data into variables (features) that a model can use. This step is critical and often requires significant domain knowledge to identify the most relevant predictors.

*   **Training and Testing:** The dataset is typically split into a **training set** (to build the model) and a **testing set** (to evaluate its performance on unseen data). This practice helps prevent **overfitting**, a common problem where the model learns the training data too well but fails to generalize to new, real-world situations.

*   **Interpretability vs. Accuracy:** Many powerful ML models (like deep neural networks) are considered "black boxes," making it difficult to understand *why* they made a particular prediction. This creates a trade-off: in social science, understanding causal mechanisms is often as important as predictive accuracy.

*   **Algorithmic Bias:** If the training data reflects existing societal biases (e.g., racial or gender biases in historical loan application data), the ML model will learn and potentially amplify those biases in its predictions. Addressing and mitigating bias is a central ethical challenge.

*   **Causality vs. Prediction:** It is crucial to remember that ML excels at prediction, but prediction does not equal causation. A model might accurately predict an outcome without revealing the underlying causal factors, which are often the primary focus of social scientific inquiry.