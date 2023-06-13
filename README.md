# OpenSearch

A Python module for simple search functionality using Levenshtein distance algorithm

## Installation

Clone the GitHub repository to your local machine:

``` console
git clone https://github.com/ArloMichael/OpenSearch.git
```

## Usage

Here is an example code snippet that demonstrates how to use `OpenSearch`:


``` python
import opensearch

db = ["hi", "how are you", "hello", "greetings"]
query = "hi"

results = opensearch.search(query, db, n=3)

print(results)
```

This will output:

``` python
['hi', 'hello', 'greetings']
```

The `search` function takes three arguments: `query` which is a string representing the search query, `db` which is a list of strings representing the database to search, and `OPTIONAL n` which limits the number of results. It returns the sorted list of items in the database based on their distance from the search query.
