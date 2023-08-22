# Intelligent_Word_Guessing_Game_using_Decision_Tree_Learning_Algorithm
The objective of this project is to design and implement a decision tree learning algorithm that can play the word-guessing game between Melbo and Melbot. The algorithm's aim is to guess the secret word chosen by Melbot within a limited number of queries, utilizing a decision tree structure to guide its guesses.

Approach:
The approach involves creating a decision tree that guides Melbo's queries to guess the secret word chosen by Melbot. The decision tree algorithm iteratively chooses the best questions to narrow down the possibilities and eventually identify the secret word. The approach includes several design decisions:

Splitting Criterion: At each internal node of the decision tree, the algorithm must determine the query word that Melbo should ask. The splitting criterion involves selecting the query word that maximizes entropy reduction. Lookahead techniques are considered, where a split resulting in maximum entropy reduction two or three levels down the tree is chosen.

Stopping Criteria: The algorithm needs to decide when to stop expanding the decision tree and make a node a leaf. Stopping criteria include a limit on the number of queries Melbo can make (Q = 15 queries per round). The tree can also be pruned if further expansion doesn't provide significant information gain.

Pruning Strategies: Pruning strategies involve removing nodes that do not contribute significantly to the decision-making process. This prevents overfitting and reduces the complexity of the decision tree.

Hyperparameters: Hyperparameters control the behavior of the decision tree algorithm, such as the depth of the tree, the minimum number of samples required to split a node, and so on. Experimentation with hyperparameters can lead to improved performance.

Lookahead: A lookahead strategy can be implemented to prioritize splits that lead to maximum entropy reduction in the future, rather than immediate gains. This strategy may be employed when the number of words in a node becomes smaller.

Alternative Metrics: Instead of entropy, the algorithm can directly aim to minimize the number of queries required to guess the secret word and increase the win rate. Different metrics can be combined to achieve a balanced split that prevents over-optimization for entropy reduction.

Impact:
The successful implementation of this decision tree learning algorithm will enable Melbo to play the word-guessing game with Melbot more effectively. The impact of the project includes:

Improved Performance: The algorithm aims to increase the number of words guessed correctly within the query limit, leading to better performance for Melbo in the word-guessing game.

Efficient Querying: The algorithm's strategic querying based on entropy reduction and lookahead techniques allows Melbo to make informed queries, leading to quicker identification of the secret word.

Algorithmic Insight: The project provides insights into decision tree learning, entropy reduction, lookahead strategies, and their applications in real-world scenarios like word-guessing games.

Customizable Solution: The algorithm can be tuned by experimenting with hyperparameters, pruning strategies, and alternative metrics to achieve optimal performance in different scenarios.

By successfully addressing the project's objectives and applying the chosen approach, the decision tree learning algorithm can significantly enhance Melbo's ability to play and win the word-guessing game against Melbot.
