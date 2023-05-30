Towards Cross Domain Recommendations: A Personality Based Probabilistic
Matrix Factorization Approach in 32nd Workshop on Information Technology and
Systems, Denmark 2022.

In this study, a novel cross-domain recommendation framework called PEMF-CD is
proposed that uses transfer learning techniques to learn personality scores from user
reviews. We achieve this by jointly embedding the text of user-generated reviews from
multiple datasets, followed by training a transformer model with personality information
to predict the personality scores of users. This approach eliminates the need for
time-consuming questionnaires and provides more practical and efficient results. The
recommendation model uses the personality-wise similarities, and rating pattern-based
similarities of users with a linear equation, supported by studies that suggest personality
has an impact on user preferences for a variety of items. The similarity scores are
incorporated into a novel probabilistic matrix factorization method that assimilates users
with similar personality scores as neighbours, wherein the users in a neighbourhood
impact each other’s recommendations to enhance the model’s accuracy.
To evaluate the proposed framework, experiments were conducted using real-world
datasets from TripAdvisor and Amazon.

Dataset: 
TripAdvisor review dataset(https://www.researchgate.net/publication/301543515_TripAdvisor_dataset_with_personality_scores/link/5718059c08aed43f63220a27/download)
Amazon magazine subscriptions dataset(https://nijianmo.github.io/amazon/index.html)

Execution order:
1. Preprocess the reviews of the dataset using preporcessing.ipynb
2. Predict the personality of amazon users from tripadvisor users with transformers
3. Perform recommendations on amazon users using PEMF
