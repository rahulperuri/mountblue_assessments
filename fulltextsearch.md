# Full Text Search

## What is full text search:
- When a search is conducted on a portion of text contained in a large body of electronically recorded text, it is referred to as a full-text search. Traditional search, on the other hand, would produce exact matches.
- Although conventional databases are excellent for storing and retrieving generic data, full-text searches have proven to be difficult. To overcome this, additional tooling is frequently needed.
- A Full-Text query allows you to search for words inside text data. Large volumes of text can be searched using full-text search. 
- A search engine might, for instance, perform a full-text search to seek for keywords across all the web pages it has indexed. Indexing is the key to this method.

## Considerations before using full text search:
- Necessary features: Adding a full-text index to your database will help you optimize text search. Still, you might need additional features such as auto-complete suggestions, synonym search, or custom scoring for relevant results.
- Architectural complexity: Adding additional software to your architecture means separate systems to maintain and additional software complexity to query two different sources.
- Costs: Whether a solution is built in-house or uses a third-party tool, additional charges are to be expected.

## Types:
1.Elastic search:
- Based on Apache Lucene, Elasticsearch is a full-text search and analytics engine. Elasticsearch allows unstructured searches like Fuzzy Searches on the stored data as well as data aggregation activities on data from many sources.
- Similar to how MongoDB handles it, it saves data in a format resembling a document. JSON representation is used for data. This adds a Non-relational nature to it and thus, it can also be used as a NoSQL/Non-relational database.

2.Solr: 
- It is an open sourced search platform which is used to develop search applications. It was built on top of lucene which is a full text search engine.Solr is enterprise-ready, fast and highly scalable.
- The applications built using Solr are sophisticated and deliver high performance. It can also be used as big data scale NOSQL database.

3.Lucene:
- Lucene is a full-text search library in Java which makes it easy to add search functionality to an application or website.It does so by adding content to a full-text index.
- It then allows you to perform queries on this index, returning results ranked by either the relevance to the query or sorted by an arbitrary field such as a document's last modified date.The content you add to Lucene can be from various sources, like a SQL/NoSQL database, a filesystem, or even from websites.

## Advantages of full text search:
- Indexing.
- Stemming.
- Weighted results.

## Disadvantages of full text search:
- Fulltext indexes can sometimes be slower to update. If the data changes a lot, there might be some lag updating indexes compared to standard indexes.
