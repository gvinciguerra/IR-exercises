# Exercises of Information Retrieval #

This repository contains the exercises (and some of their solutions) of the
various test exams of the Information Retrieval (IR) course, taught by prof.
Paolo Ferragina.

## Subjects of the course ##

Like the course, the various solutions will be divided into the following topics:

  1. **Introduction**: Boolean retrieval model. Matrix document-term. Inverted list: dictionary + postings. How to implement an AND, OR and NOT queries, and their time complexities.
  2. **Crawling**: Mercator, Bloom Filters, Consistent Hashing, Web graph.
  3. **Locality-Sensitive Hashing**: K-means, Hamming distance, Locality Sensitive Hashing (LSH).
  4. **Documents Compression**: Compressed storage of documents: LZ-based compression. Storage and Transmission of single/group of file(s): Delta compression (Zdelta), File Synchronization (rsync, zsync), and Set Reconciliation.
  5. **Parsing and Text Laws**: Parsing: tokenization, normalization, lemmatization, stemming, thesauri. Statistical properties of texts: Zipf law: classical and generalized, Heaps law, Luhn's consideration.
  6. **Index Construction**: The issue of hierarchical memories: I/O-model. Index construction: multi-way mergesort, BSBI and SPIMI. Sketch on MapReduce. Distributed indexing: Term-based vs Doc-based partitioning. Dynamic indexing: two indexes, a cascade of indexes.
  7. **Postings Compression**: Posting list compression, codes: gamma, delta, variable bytes, PForDelta and Elias-Fano. Rank and Select data structures, two approaches: the case of B untouched and extra o(B) bits, and the case of Elias-Fano's approach with B compressed. Succinct representation of binary trees and its navigational operations (heap like notation).
  8. **Dictionary Search**: Exact search: hashing with chaining, univeral hashing, cuckoo hashing. Prefix search: compacted trie, front coding, 2-level indexing. Edit distance via brute-force approach, or Dynamic Programming (possibly weighted). Overlap measure with k-gram index. Edit distance with k-gram index. One-error match. Wild-card queries (permuterm, k-gram). Phonetic match. Context-sensitive match.
  9. **Query Resolver**: Query processing: skip pointers (with solution based on dynamic programming), caching, phrase queries. Zone index and tiered index. The auto-complete problem and its solutions for the top-1, top-2, ..., top-k strings.
  10. **Text Ranking**: Text-based ranking: dice, jaccard, tf-idf. Vector space model. Storage of tf-idf and use for computing document-query similarity. Fast top-k retrieval: high idf, champion lists, many query-terms, fancy hits, clustering. Exact Top-K: WAND and blocked-WAND. Relevance feedback, Rocchio, pseudo-relevance feedback, query expansion. Performance measures: precision, recall, F1 and user happiness.
  11. **Web Ranking**: Random Walks. Link-based ranking: pagerank, topic-based pagerank, personalized pagerank, CoSim rank.
  12. **Applications**: HITS. Recommendation systems and Web advertising.
  13. **Projections**: Projections to smaller spaces: Latent Semantic Indexing (LSI). Random Projections: Johnson-Linderstauss Lemma and its applications.
  14. **Topic Annotator**: Semantic-annotation tools: basics, Wikipedia structure, TAGME and other annotators. How to evaluate those systems.
  15. **Lucene**: Introduction to Lucene.

## Topics-by-date Table ##

In this table is shown which kind of exercises you may find in a specific test exam (denoted by the date in which it was taken). The numbers describe the topics as in the previous section.

***WARNING***: The following table is just a stub. Many exercises may be misclassified.

***WARNING***: Every exam taken before 2016 may contain exercises form a previous programme.

| Test Date                                                                                                  | 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 | 9 | 10| 11| 12| 13| 14| 15| Status                                                     |
|:----------------------------------------------------------------------------------------------------------:|:-:|:-:|:-:|:-:|:-:|:-:|:-:|:-:|:-:|:-:|:-:|:-:|:-:|:-:|:-:|:----------------------------------------------------------:|
| [05/09/17](http://didawiki.di.unipi.it/lib/exe/fetch.php/magistraleinformatica/ir/ir16/ir170905.docx)      |   |   |   | ● |   | ● |   | ● |   |   | ● |   |   |   |   |![Status](https://img.shields.io/badge/Solved-0%2F4-red.svg)|
| [27/07/17](http://didawiki.di.unipi.it/lib/exe/fetch.php/magistraleinformatica/ir/ir16/ir170727.docx)      |   |   |   |   |   |   | ● | ● |   | ● | ● |   |   |   | ● |![Status](https://img.shields.io/badge/Solved-0%2F6-red.svg)|
| [29/06/17](http://didawiki.di.unipi.it/lib/exe/fetch.php/magistraleinformatica/ir/ir16/ir170629.docx)      |   |   |   |   |   |   | ● | ● |   | ● | ● |   |   |   | ● |![Status](https://img.shields.io/badge/Solved-0%2F5-red.svg)|
| [12/06/17](http://didawiki.di.unipi.it/lib/exe/fetch.php/magistraleinformatica/ir/ir16/ir170612.docx)      |   |   |   |   |   | ● | ● |   |   | ● | ● |   |   | ● | ● |![Status](https://img.shields.io/badge/Solved-0%2F5-red.svg)|
| [01/02/17](http://didawiki.di.unipi.it/lib/exe/fetch.php/magistraleinformatica/ir/ir16/ir170201_lab.docx)  |   |   |   |   |   |   |   |   |   |   |   |   |   |   | ● |![Status](https://img.shields.io/badge/Solved-0%2F2-red.svg)|
| [12/01/17](http://didawiki.di.unipi.it/lib/exe/fetch.php/magistraleinformatica/ir/ir16/ir170112.docx)      |   | ● | ● | ● |   |   |   |   |   | ● | ● |   |   |   |   |![Status](https://img.shields.io/badge/Solved-0%2F6-red.svg)|
| [10/01/17](http://didawiki.di.unipi.it/lib/exe/fetch.php/magistraleinformatica/ir/ir16/ir170110_lab.docx)  |   |   |   |   |   |   |   |   |   |   |   |   |   |   | ● |![Status](https://img.shields.io/badge/Solved-0%2F2-red.svg)|
| [02/09/16](http://didawiki.di.unipi.it/lib/exe/fetch.php/magistraleinformatica/ir/ir15/ir160902.docx)      |   | ● | ● | ● |   |   |   | ● |   |   |   |   |   |   |   |![Status](https://img.shields.io/badge/Solved-0%2F5-red.svg)|
| [27/06/16](http://didawiki.di.unipi.it/lib/exe/fetch.php/magistraleinformatica/ir/ir15/ir160627.docx)      |   | ● |   |   |   |   | ● | ● |   |   | ● |   |   |   |   |![Status](https://img.shields.io/badge/Solved-0%2F4-red.svg)|
| [01/02/16](http://didawiki.di.unipi.it/lib/exe/fetch.php/magistraleinformatica/ir/ir15/ir160201.docx)      |   |   | ● | ● |   |   |   | ● |   | ● |   |   |   | ● |   |![Status](https://img.shields.io/badge/Solved-0%2F6-red.svg)|
| [11/01/16](http://didawiki.di.unipi.it/lib/exe/fetch.php/magistraleinformatica/ir/ir15/ir160111.docx)      |   |   | ● | ● |   |   | ● | ● |   |   | ● |   |   | ● |   |![Status](https://img.shields.io/badge/Solved-0%2F6-red.svg)|
| [10/09/15](http://didawiki.di.unipi.it/lib/exe/fetch.php/magistraleinformatica/ir/ir14/ir150910.docx)      |   | ● |   | ● |   |   |   | ● |   | ● |   |   |   |   |   |![Status](https://img.shields.io/badge/Solved-0%2F6-red.svg)|
| [20/07/15](http://didawiki.di.unipi.it/lib/exe/fetch.php/magistraleinformatica/ir/ir14/ir150720.docx)      |   |   |   |   |   |   |   |   |   | ● |   |   |   |   |   |![Status](https://img.shields.io/badge/Solved-0%2F5-red.svg)|
| [29/06/15](http://didawiki.di.unipi.it/lib/exe/fetch.php/magistraleinformatica/ir/ir14/ir150629.docx)      |   | ● |   |   |   |   |   |   |   | ● |   |   |   | ● |   |![Status](https://img.shields.io/badge/Solved-0%2F4-red.svg)|
| [05/06/15](http://didawiki.di.unipi.it/lib/exe/fetch.php/magistraleinformatica/ir/ir14/ir150605.docx)      |   |   |   |   |   |   | ● |   |   | ● | ● |   | ● |   |   |![Status](https://img.shields.io/badge/Solved-0%2F5-red.svg)|
| [09/02/15](http://didawiki.di.unipi.it/lib/exe/fetch.php/magistraleinformatica/ir/ir14/ir150209.docx)      |   |   |   |   |   |   |   | ● |   | ● |   |   |   |   |   |![Status](https://img.shields.io/badge/Solved-0%2F4-red.svg)|
| [16/01/15](http://didawiki.di.unipi.it/lib/exe/fetch.php/magistraleinformatica/ir/ir14/ir150116.docx)      | ● |   |   |   |   |   |   | ● |   |   |   |   |   |   |   |![Status](https://img.shields.io/badge/Solved-0%2F5-red.svg)|
| [29/06/14](http://didawiki.di.unipi.it/lib/exe/fetch.php/magistraleinformatica/ir/ir13/ir140729.docx)      |   |   |   |   |   | ● |   | ● |   |   |   |   |   |   |   |![Status](https://img.shields.io/badge/Solved-0%2F4-red.svg)|
| [30/06/14](http://didawiki.di.unipi.it/lib/exe/fetch.php/magistraleinformatica/ir/ir13/ir140630.docx)      |   |   |   |   |   |   |   |   |   |   |   |   |   |   |   |![Status](https://img.shields.io/badge/Solved-0%2F4-red.svg)|
| [09/06/14](http://didawiki.di.unipi.it/lib/exe/fetch.php/magistraleinformatica/ir/ir13/ir140609.docx)      |   |   |   |   |   |   |   | ● | ● |   |   |   |   |   |   |![Status](https://img.shields.io/badge/Solved-0%2F5-red.svg)|
| [29/01/14](http://didawiki.di.unipi.it/lib/exe/fetch.php/magistraleinformatica/ir/ir13/ir140129.docx)      |   |   |   |   |   |   | ● | ● |   |   |   |   | ● |   |   |![Status](https://img.shields.io/badge/Solved-0%2F6-red.svg)|
| [08/01/14](http://didawiki.di.unipi.it/lib/exe/fetch.php/magistraleinformatica/ir/ir13/ir140108.docx)      |   | ● |   |   |   |   | ● | ● | ● |   |   |   |   |   |   |![Status](https://img.shields.io/badge/Solved-0%2F6-red.svg)|
| [16/07/13](http://didawiki.di.unipi.it/lib/exe/fetch.php/magistraleinformatica/ir/ir12/ir130716.docx)      |   |   |   |   |   |   |   | ● |   |   |   |   |   |   |   |![Status](https://img.shields.io/badge/Solved-0%2F6-red.svg)|
| [25/06/13](http://didawiki.di.unipi.it/lib/exe/fetch.php/magistraleinformatica/ir/ir12/ir130625.docx)      |   |   |   |   |   |   |   |   |   | ● | ● |   |   |   |   |![Status](https://img.shields.io/badge/Solved-0%2F5-red.svg)|
| [12/02/13](http://didawiki.di.unipi.it/lib/exe/fetch.php/magistraleinformatica/ir/ir12/ir130212.docx)      |   |   |   |   |   |   |   |   |   | ● |   |   |   |   |   |![Status](https://img.shields.io/badge/Solved-0%2F6-red.svg)|
| [10/01/13](http://didawiki.di.unipi.it/lib/exe/fetch.php/magistraleinformatica/ir/ir12/ir130110.docx)      |   |   | ● |   |   |   |   | ● |   |   |   |   | ● |   |   |![Status](https://img.shields.io/badge/Solved-0%2F6-red.svg)|
| [03/09/12](http://didawiki.di.unipi.it/lib/exe/fetch.php/magistraleinformatica/ir/ir11/ir120903.doc)       |   |   |   |   |   |   |   | ● |   | ● |   |   |   |   |   |![Status](https://img.shields.io/badge/Solved-0%2F4-red.svg)|
| [23/07/12](http://didawiki.di.unipi.it/lib/exe/fetch.php/magistraleinformatica/ir/ir11/ir120723.doc)       |   | ● |   |   |   |   |   |   |   |   | ● |   |   |   |   |![Status](https://img.shields.io/badge/Solved-0%2F4-red.svg)|
| [08/06/12](http://didawiki.di.unipi.it/lib/exe/fetch.php/magistraleinformatica/ir/ir11/ir120608.doc)       |   |   |   |   | ● |   |   |   |   | ● |   |   |   |   |   |![Status](https://img.shields.io/badge/Solved-0%2F5-red.svg)|
| [01/02/12](http://didawiki.di.unipi.it/lib/exe/fetch.php/magistraleinformatica/ir/ir11/ir120201.doc)       |   |   |   |   |   |   |   | ● |   |   |   |   |   |   |   |![Status](https://img.shields.io/badge/Solved-0%2F5-red.svg)|
| [11/01/12](http://didawiki.di.unipi.it/lib/exe/fetch.php/magistraleinformatica/ir/ir11/ir120111.doc)       |   |   |   |   |   |   |   | ● |   | ● |   |   |   |   |   |![Status](https://img.shields.io/badge/Solved-0%2F3-red.svg)|
| [07/12/11](http://didawiki.di.unipi.it/lib/exe/fetch.php/magistraleinformatica/ir/ir11/ir111207.doc)       | ● |   |   |   |   |   |   |   |   |   |   |   |   |   |   |![Status](https://img.shields.io/badge/Solved-0%2F4-red.svg)|
| [01/09/11](http://didawiki.di.unipi.it/lib/exe/fetch.php/magistraleinformatica/ir/ir10/ir110901.doc)       | ● | ● |   |   |   |   |   |   |   | ● |   |   |   |   |   |![Status](https://img.shields.io/badge/Solved-0%2F6-red.svg)|
| [20/07/11](http://didawiki.di.unipi.it/lib/exe/fetch.php/magistraleinformatica/ir/ir10/ir110720.doc)       |   |   |   |   |   |   |   |   |   |   |   |   |   |   |   |![Status](https://img.shields.io/badge/Solved-0%2F6-red.svg)|
| [24/06/11](http://didawiki.di.unipi.it/lib/exe/fetch.php/magistraleinformatica/ir/ir10/ir110624.doc)       |   |   |   |   |   |   | ● | ● |   |   |   |   |   |   |   |![Status](https://img.shields.io/badge/Solved-0%2F6-red.svg)|
| [21/02/11](http://didawiki.di.unipi.it/lib/exe/fetch.php/magistraleinformatica/ir/ir10/ir110221.doc)       |   |   |   |   |   |   |   | ● |   |   |   |   |   |   |   |![Status](https://img.shields.io/badge/Solved-0%2F4-red.svg)|
| [01/02/11](http://didawiki.di.unipi.it/lib/exe/fetch.php/magistraleinformatica/ir/ir10/ir110201.doc)       |   | ● |   |   |   |   |   |   |   |   |   |   |   |   |   |![Status](https://img.shields.io/badge/Solved-0%2F4-red.svg)|
