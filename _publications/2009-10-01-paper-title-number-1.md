---
title: "Layered Neighborhood Expansion for Incremental Multiple Graph Matching"
collection: publications
permalink: /publication/2009-10-01-paper-title-number-1
excerpt: 'multi-graph matching, clustering, self-supervised learning'
date: 2020-08-23
venue: 'ECCV 2020'
paperurl: 'https://link.springer.com/chapter/10.1007/978-3-030-58607-2_15'
citation: 'Chen Z, Xie Z, Yan J, et al. Layered neighborhood expansion for incremental multiple graph matching[C]//Computer Vision–ECCV 2020: 16th European Conference, Glasgow, UK, August 23–28, 2020, Proceedings, Part X 16. Springer International Publishing, 2020: 251-267.'
---

**Abstract**
Graph matching has been a fundamental problem in computer vision and pattern recognition, for its practical flexibility as well as NP hardness challenge. Though the matching between two graphs and among multiple graphs have been intensively studied in literature, the online setting for incremental matching of a stream of graphs has been rarely considered. In this paper, we treat the graphs as graphs on a super-graph, and propose a novel breadth first search based method for expanding the neighborhood on the super-graph for a new coming graph, such that the matching with the new graph can be efficiently performed within the constructed neighborhood. Then depth first search is performed to update the overall pairwise matchings. Moreover, we show our approach can also be readily used in the batch mode setting, by adaptively determining the order of coming graph batch for matching, still under the neighborhood expansion based incremental matching framework. Experiments on both online and offline matching of graph collections show our approach's state-of-the-art accuracy and efficiency.

