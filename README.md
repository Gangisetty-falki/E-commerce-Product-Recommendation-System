# E-commerce-Product-Recommendation-System
# Product-recommendation-e-commerce system
In order to offer users customized product recommendations based on their browsing and purchase history, I developed an e-commerce product recommendation system. This system analyzes user activity and generates recommendations using content-based filtering algorithms and collaborative filtering, which improves the shopping experience and increases revenue for e-commerce enterprises.

### Set of data
I assigned unique identities to an Amazon dataset of customer ratings for electronic devices in order to prevent biases. The Amazon Electronics Rating Dataset Recommendation is a dataset that can be downloaded [here](https://www.kaggle.com/datasets/vibivij/download?datasetVersionNumber=1).

### Methodology

1. **Rank-Based Product Recommendation** - **Objective**: Solve the Cold Start Problem and suggest the most well-liked products to prospective clients.
   - **Action**: Determine the overall number of ratings and the average rating for every product. Offer the best products with the required number of minimal interactions.
2. **Similarity-Based Collaborative Filtering** - **Objective**: Offer tailored suggestions derived from comparable users' exchanges.
   - **Action**: Transform user IDs into integers, utilize cosine similarity to identify similar users, and suggest products that similar users have used but the actual user has not.

3. **Model-Based Collaborative Filtering** - **Objective**: Offer individualized suggestions based on prior actions and preferences, taking sparsity and scalability into consideration.
   - **Action**: To minimize dimensionality, predict ratings, and suggest top goods based on predicted ratings, use SVD to a CSR matrix of product ratings.
   **Evaluation**: By comparing actual and anticipated ratings, compute the root mean square error (RMSE) to assess model performance.
