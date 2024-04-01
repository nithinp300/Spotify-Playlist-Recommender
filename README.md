# Spotify Playlist Recommender

### Spotify Million Playlist Dataset Challenge

#### Task Description
The challenge aims to develop a system for automatic playlist continuation. Given a user-created playlist, the system should generate a list of recommended tracks to add to the playlist, continuing its theme. The input includes playlist metadata and a variable number of seed tracks (0, 1, 5, 10, 25, or 100), and the output should be a list of 500 recommended candidate tracks ordered by relevance.

#### Dataset
The Million Playlist Dataset (MPD) consists of 1,000,000 playlists created by users on Spotify. Each playlist contains metadata, track lists, editing information, and other details. The dataset is divided into 1,000 slice files, each containing 1,000 playlists.

#### Evaluation Metrics
Submissions will be evaluated using several metrics, including R-precision, Normalized Discounted Cumulative Gain (NDCG), and Recommended Songs clicks. These metrics measure the accuracy and relevance of the recommended tracks.

#### Proposed Solutions
- Collaborative Filtering: Using similarity between playlists or songs to predict track recommendations based on past user behavior.
- K Nearest Neighbor: Using playlist or song similarities to recommend tracks based on nearest neighbors.
- Frequent Pattern Growth: Mining frequent patterns in playlists to recommend tracks.
- Word2Vec: Utilizing Word2Vec embeddings to capture track relationships and recommend similar tracks.

#### Challenges
- Large Dataset: The dataset contains 1 million playlists and over 66 million tracks, which may require substantial computational resources.
- Algorithm Complexity: Some recommender algorithms, such as collaborative filtering and matrix factorization, can be complex and computationally intensive.

#### Preliminary Results
- Playlist-based CF: Achieved an R-precision of 0.621 with top K rating songs.
- Song-based CF: Achieved an R-precision of 0.7847 with baseline methods.
- Word2Vec + Playlist-based: Achieved an R-precision of 0.0190 with Word2Vec embeddings.

#### Conclusion
The challenge of automatic playlist continuation involves developing effective recommender systems to suggest relevant tracks for playlists. Various approaches, including collaborative filtering, K Nearest Neighbor, and Word2Vec, can be used to address this task, with each method offering its own advantages and challenges.