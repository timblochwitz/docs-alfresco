---
title: Alfresco Search Enterprise
---

Alfresco Content Services supports the Elasticsearch platform for searching within the repository using Alfresco Search Enterprise 3.0.

[Elastic Search](https://www.elastic.co/guide/en/elasticsearch/reference/current/elasticsearch-intro.html){:target="_blank"} is an open source enterprise search platform that uses the [Lucene](https://lucene.apache.org/){:target="_blank"} engine for indexing and searching. Elasticsearch is written in Java and runs as a standalone search server. The Alfresco Repository sends HTTP requests to Elasticsearch to search for content and metadata. The Alfresco Elasticsearch Connector updates the cores and indexes in Elasticsearch. This consumes ActiveMQ messages produced by the Alfresco Repository when folders, documents, and permissions are created or updated in the repository.

> **Note:** The *alfresco* index is the only index in Elasticsearch used for searching live content. The index used for content marked as deleted (named *archive* in previous versions) is not available when using Elasticsearch.

The **Search** feature is provided by the Alfresco Repository itself which communicates with the Elasticsearch server that then performs the required format translation for queries and results. The Elasticsearch index contains all the content, metadata, and permissions for a single document, so no external Elasticsearch plugin is required.

The **Indexing** feature is provided by a Spring Boot application called `Alfresco Elasticsearch Connector`. The application is split into two main components called **Live Indexing** and **Re-indexing**, for more information see [Indexing]({% link search-enterprise/latest/admin/index.md %}#elastic-search-connector).

Alfresco Search Enterprise consists of the following components:

* Alfresco Content Services 7.1
* Elasticsearch 7.10. (It can be used as a standard managed service or can be installed using default configuration)
* Alfresco Elasticsearch Connector 3.0

The services required for Search Enterprise are included in the following diagram.

![architecture]({% link search-enterprise/images/elasticsearch_connector_architecture.png %})