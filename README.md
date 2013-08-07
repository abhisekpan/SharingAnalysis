SharingAnalysis
===============================================================================
A Pintool to analyze different facets of sharing among the threads of a shared-
memory multithreaded application. Analysis of data-sharing can be useful in
many areas of multi-core processor design, such as shared cache management and
coherence optimization.

Objectives
-------------------------------------------------------------------------------
The tool has following objectives:

* Temporal nature of sharing.  
When a data element is shared ie. it is accessed by multiple cores, we want to
know the number of unique accesses that happen between each shared reuse. This
is important because if shared reuse is too high, then the chance that the 
entry will be evicted before reuse goes up and partitioned caches become a 
better choice than a globally replaced cache.
* Extent of sharing among threads.  
Percent of references that are accessed by only 1 thread, 2 threads, and so on.

* Shared vs. private accesses for an address.  
For each address, what percent of time the access is shared and what percent
of time the access is private. A shared access means two consecutive accesses
from 2 different threads, and a private access means two consecutive accesses
from the same thread.
* Temporal distribution of communication events.

Performance Improvement
-------------------------------------------------------------------------------
Sampling.

Visualization
-------------------------------------------------------------------------------

