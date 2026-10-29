# Project-Deliverable-2
How to read: Run all cells in order from top to bottom.

Code organization:

Pre-processing (Cells 1-7):

We explored our data to gain a better understanding and then split our data into a training dataset, dev dataset, and test dataset.

The split uses random_state=67 to make sure the split stays the same when running the cells.

We split each ingredient list on commas, removed the brackets, all apostrophes, all quotes, and all leading and trailing spaces and treated each ingredient as a single token even if it contained multiple words.

Example:
 "ingredients": [ "penne pasta",  "grated parmesan cheese", "ground beef", "shredded mozzarella cheese","garlic sauce" ]
The list above contains 5 tokens/ingredients.


Training (train and dev set):

Format: Cell #: [model name]

Cell # refers to its position in the notebook, which starts from 1 and not the execution number in [].

Cell 8: Baseline model

Cell 9-10: Individual words model

Cell 11: Prep word model

Cell 12: Common word model

Cell 13: Individual words + prep word model

Testing (test set):

Cell 14: Testing baseline model (accuracy, precision, recall, f1-score)

Evaluation (test set):

Cell 15: Full confusion matrix for baseline model

Cell 16: 2x2 confusion matrix for each cuisine in baseline model

Cell 17: Pooled confusion matrix, microaveraged and macroaveraged precision

Cell 18: Top 5 most informative features for each cuisine
