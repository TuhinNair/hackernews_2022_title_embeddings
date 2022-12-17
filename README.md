# hackernews_2022_title_embeddings

For more information on how I used these embeddings, refer to this blog post: [Market research using GPT-3 and Hacker News](https://idiotlamborghini.com/articles/)

- The `title_embeddings` folder contains 51,275 vectors of 4096 dimensions each.
  - Created using OpenAI's `text-search-curie-doc-001` model.
  - Uses just the title string from Hacker News posts. The posts:
    - had at least 10 points
    - at least one comment
    - and were made between the start of 2022 and 5PM UTC on Dec 9th, 2022.
  - Each file is in the format `<item_id>.json` where the item id corresponds to the id returned by the [Hacker News API](https://github.com/HackerNews/API#items)

- The `search_query_embeddings` folder contains a few example query vectors created using OpenAI's `text-search-curie-query-001` model.