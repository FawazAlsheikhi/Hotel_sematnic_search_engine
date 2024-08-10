
# Semantic Hotel Search

**By:** 

@Fawaz Alsheikhi

@Taif Alharbi

@Nora .....

**Description:**  
This project implements a semantic search system designed to identify the most relevant hotels based on a user query. By leveraging advanced natural language processing techniques, the notebook ranks hotels according to their relevance to the input query, considering both similarity and sentiment.

<div align="center">
   
![User serach](qurey.png)

![Luxury Hotel in London](qurey_output.png)

</div>

**Key Features:**
- **Semantic Search:** Utilizes deep learning models to perform semantic search, ensuring that hotel recommendations closely match the intent and context of the user’s query.
- **City Extraction:** The `extract_city` function identifies and extracts city names from user queries to filter the search space.
- **Similarity and Sentiment Ranking:** The notebook includes functions like `filter_and_rank_by_similarity` and `filter_and_rank_by_similarity_sentiment_ranking`, which rank hotels based on their similarity to the query and their sentiment score.

**Functions:**

1. **`extract_city(query, cities):`**  
   Extracts the city from the query based on a provided list of cities.

2. **`filter_and_rank_by_similarity(query, df, model, cities):`**  
   Filters and ranks hotel results by their semantic similarity to the user query within a given DataFrame.

3. **`filter_and_rank_by_similarity_sentiment_ranking(query, df, model, cities, k):`**  
   Ranks hotels by both semantic similarity and sentiment, returning the top `k` most relevant hotels.

4. **`gr_request(query):`**  
   (Description needed: Please clarify what this function does.)

**Dependencies:**
- Python 3.x
- Required libraries:
  - NumPy
  - Pandas
  - TensorFlow/PyTorch (or another NLP framework)
  - Any other relevant libraries for NLP and semantic search

**Installation:**
Install the required dependencies using:
```bash
pip install -r requirements.txt
```

**Usage:**
To use the semantic search functions:
1. **Run the notebook:** Execute the notebook to load all functions and dependencies.
2. **Search for hotels:** Call the functions to perform semantic search based on a user query. For example:
   ```python
   relevant_hotels = filter_and_rank_by_similarity(query, df, model, cities)
   ```
3. **Refine results by sentiment:** Use the sentiment ranking function for more tailored results:
   ```python
   top_hotels = filter_and_rank_by_similarity_sentiment_ranking(query, df, model, cities, k)
   ```

**Examples:**
Provide examples of typical queries and the resulting hotel recommendations, demonstrating the effectiveness of the semantic search.

**Contributing:**
If you wish to contribute to this project, please follow these guidelines:
- Fork the repository.
- Create a new branch (`git checkout -b feature-branch`).
- Commit your changes (`git commit -am 'Add new feature'`).
- Push to the branch (`git push origin feature-branch`).
- Create a new Pull Request.

**License:**
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
