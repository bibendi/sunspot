Copyright transaxtions llc, Pleasanton, CA 94588
Ver 3.5 with NRT uses RankingAlgorithm ver 1.3

Dec 11, 2011

Solr 3.5 with Ranking Algorithm 1.3 (NRT support)
-------------------------------------------------
For license information, LICENSE_SOLR_RA.txt

For more info on Solr with RankingAlgorithm, see http://solr-ra.tgels.com/solr-ra.jsp

For more info on Ranking Algorithm, see http://ra.tgels.com/rankingalgorithm.jsp

For install and starting Solr with RA info, see http://solr-ra.tgels.com/solr-ra-install.jsp

Solr with RA white paper available at http://solr-ra.tgels.com/papers/Solr_with_RankingAlgorithm.pdf


Starting Solr with RA
----------------------
It should be the same as before. Change to examples directory and run
java -jar start.jar or use the start_solr.sh script.

Creating an Index and Searching
-------------------------------
You should be able to create and search the index as before, no changes.
By default, RankingAlgorithm is enabled. If you want to use the Lucene 
library, add lucene=true to the query or change library attribute in
solr/conf/solconfig.xml.

Testing
-------

Try http://localhost:8983/solr/select/?q=john

For faceting:
http://localhost:8983/solr/select/?q=john&facet=on&facet.field=a_name&facet.field=a_type

see: http://solr-ra.tgels.com/wiki/en/Near_Real_Time_Search

Note: 

1.This release includes the mbartists index, about 390k documents. [do a search with *:* to get the contents]




