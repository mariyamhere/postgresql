# PostgreSQL for 3 Different Use Cases

## The E-Commerce Product Catalog (Best for Hybrid Search)

To test pgvector's true super-power, I combined traditional SQL filters with vector similarity (e.g., "Find the 5 products most semantically similar to 'comfortable running shoes' under $100"). Dataset used: [Amazon All Categories Best Sellers + Reviews](https://www.kaggle.com/datasets/tigboatnc/amazon-all-categories-best-sellers-reviews)

This dataset got short-to-medium descriptions, and I needed blazing-fast response times on a standard CPU, and so I preferred the _multilingual-e5-small_ embedding model. It's open-source and suport multilingual search, and runs offline.

