# Pages-You-Might-like-Recommendation
Pages You Might Like – A Python-based recommendation system that suggests pages to users based on shared interests with other users. Ideal for learning simple recommendation algorithms for social networks and content discovery.

# Pages You Might Like Recommendation System

A Python project that recommends pages to users based on the pages liked by other users with similar interests. Inspired by social media platforms, it identifies content a user might enjoy based on shared interactions.

## Features

- Loads user and page data from a JSON file (`data.json`)
- Computes page recommendations based on shared interests
- Ranks suggested pages by the number of shared interactions
- Lightweight and easy to extend

## Dataset

The project uses a JSON structure with:

- **Users**: Each user has an `id`, `name`, list of `friends`, and `liked_pages`
- **Pages**: Pages that users like

Example snippet of `data.json`:

```json
{
    "users": [
        {"id": 1, "name": "Amit", "friends": [2, 3], "liked_pages": [101]},
        {"id": 2, "name": "Priya", "friends": [1, 4], "liked_pages": [102]}
    ],
    "pages": [
        {"id": 101, "name": "Python Developers"},
        {"id": 102, "name": "Data Science Enthusiasts"}
    ]
}
```
# How It Works
1. Load user data from data.json
2. For a given user, identify pages liked by other users
3. Compare shared interests to determine pages the user might like
4. Recommend pages ranked by the number of shared interactions

# Future Enhancements
Include friend network influence in recommendations
Build a small web interface for page suggestions
Implement collaborative filtering algorithms

