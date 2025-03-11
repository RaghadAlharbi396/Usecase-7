# Usecase-7

## to test modele deployment try this:
### for supervised ML (Knn):
curl -X POST "[https://model-deploymant-unsupervised.onrender.com/predict](https://model-deplymant-supervised.onrender.com/predict)" \
-H "Content-Type: application/json" \
-d '{
    "appearance": 30,
    "minutes_played": 1500,
    "games_injured": 3,
    "award": 1,
    "highest_value": 5000000.0
}'
### for unsupervised ML (Kmeans):
curl -X POST "https://model-deploymant-unsupervised.onrender.com/predict" \
-H "Content-Type: application/json" \
-d '{
  "appearance": 25,
  "minutes_played": 1200,
  "highest_value": 15.5
}'
