# Elasticsearch Indexing

Elasticsearch is a powerful full-text search platform. It offers great flexibility to analyze and index data the way **you** want. The flexibility is a great feature of the platform but can be daunting for developers when getting started.

As developers, we have a common cross-section of data points that may exist in our datasets. For example:

- Names
- Emails
- Phone Numbers
- Identifiers (Guids, Numeric, or Alphanumeric)
- Web Addresses
- Physical Addresses

The conversation will walk through each data point and answer the following questions:

> How does a User want to search for the particular data point?

> How should we store and analyze the data point?

> How should we analyze the search input (if applicable)?

> How do we create a `global` search query that boosts relevant fields appropriately?

By the end of the conversation, we should have produced the following:

- An index mapping
- An analyzer for each kind of input (based on our discussion)

We can assume we will be using the latest version Elasticsearch at the time, which is `5.6.1`. We will also be using the [`accounts`](https://download.elastic.co/demos/kibana/gettingstarted/accounts.zip) sample dataset provided by **Elastic**.
