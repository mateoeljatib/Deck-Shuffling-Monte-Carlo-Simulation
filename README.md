# Deck-Shuffling-Monte-Carlo-Simulation
Monte Carlo simulation of a card shuffling method to analyze positional biases

This project simulates the shuffling of a deck of 40 cards using a Monte Carlo approach. The goal is to analyze whether a specific card (Card 1) has an equal probability of ending up in any position after shuffling. The method used attempts to mimic a real-world shuffle process by repeatedly splitting and interleaving the deck in a structured yet random manner.

How the Simulation Works:

- Deck Initialization: A deck of 40 cards, numbered 1 to 40, is created in order.

- Gaussian-Based Cutting: A portion of the deck is split using a Gaussian probability distribution centered around position 20, ensuring the cut point falls between the 15th and 25th cards.

Interleaving Shuffle:

- The second half of the deck is divided into 2 to 4 parts of roughly equal size.

- These parts are interleaved with the first half.

Repeated Shuffling: The process is repeated randomly between 4 and 8 times to simulate a real-world shuffle.

Monte Carlo Analysis: The shuffle is executed 500 to 1000 times, tracking where Card 1 ends up after each run.

Statistical Testing:

- A histogram is generated to visualize the final positions of Card 1.

- A chi-square test is performed to determine if the final distribution deviates significantly from a uniform distribution.

Results & Observations:

- If the shuffle is perfectly uniform, each position should have approximately equal probability.

- If the shuffle is biased, certain positions will be overrepresented.

- The chi-square test helps assess whether the observed distribution is significantly different from a uniform one.
