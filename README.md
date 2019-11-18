# Elastic_Sandbox  <BR/>
Tutorial repository for personal enrichment<p>
FROM: Elasticsearch</p>elastic/elasticsearch<br/>
h1. Elasticsearch

h2. A Distributed RESTful Search Engine

h3. "https://www.elastic.co/products/elasticsearch":https://www.elastic.co/products/elasticsearch

Elasticsearch is a distributed RESTful search engine built for the cloud. Features include:

* Distributed and Highly Available Search Engine.
** Each index is fully sharded with a configurable number of shards.
** Each shard can have one or more replicas.
** Read / Search operations performed on any of the replica shards.
* Multi Tenant.
** Support for more than one index.
** Index level configuration (number of shards, index storage, ...).
* Various set of APIs
** HTTP RESTful API
** Native Java API.
** All APIs perform automatic node operation rerouting.
* Document oriented
** No need for upfront schema definition.
** Schema can be defined for customization of the indexing process.
* Reliable, Asynchronous Write Behind for long term persistency.
* (Near) Real Time Search.
* Built on top of Lucene
** Each shard is a fully functional Lucene index
** All the power of Lucene easily exposed through simple configuration / plugins.
* Per operation consistency
** Single document level operations are atomic, consistent, isolated and durable.

h2. Getting Started

First of all, DON'T PANIC. It will take 5 minutes to get the gist of what Elasticsearch is all about.

h3. Requirements

You need to have a recent version of Java installed. See the "Setup":http://www.elastic.co/guide/en/elasticsearch/reference/current/setup.html#jvm-version page for more information.

h3. Installation

* "Download":https://www.elastic.co/downloads/elasticsearch and unzip the Elasticsearch official distribution.
* Run @bin/elasticsearch@ on unix, or @bin\elasticsearch.bat@ on windows.
* Run @curl -X GET http://localhost:9200/@.
* Start more servers ...
