# Youtube-Video-Likes-Predictor
This project uses a deep learning neural network to predict the likes-to-views ratio of a YouTube video.

YouTube is one of the largest video-sharing platforms, where content creators rely on audience engagement metrics such as likes, views, and comments to measure their success. Deep learning can analyze large-scale YouTube metadata, video features, and historical engagement trends to build a predictive model that estimates the number of likes a video will receive. This can help creators optimize their content strategy, improve audience engagement, and increase monetization opportunities. This is also a useful tool for brands to analyze and strategically place their YouTube ads.


Below is a summary and inference derived after implementing, training, and testing the model:
1. The YouTube Likes Predictor model was trained on a cleaned and engineered dataset that combined video metadata, text features, and engagement metrics.
2. After applying TF-IDF on video titles, descriptions, and tags, and reducing dimensionality using PCA, the final FFNN model was trained using L1 loss.
3. During training, the model’s validation loss gradually decreased, showing stable learning.
4. The final model achieved good performance in predicting the like-to-view ratio, with the lowest average validation loss of 0.039 using the Adam optimizer.
5. The addition of text features (via TF-IDF) and new categorical features like language presence (e.g., Arabic, Hindi) helped improve prediction accuracy.
6. However, handling highly skewed engagement data remained challenging, especially for videos with extreme outliers in views or comments.
