# Configurations
Different configurations for Quicksearch and FindIt

Note that there are 2 sets of production configurations for Quicksearch under main:
- Ingest configs optimized for indexing on app2
- Search configs optimized for search on app1 and app3

# NOTE
- Quicksearch Solr Docker Configure is pull from the repo: https://git.yale.edu/Library-IT/quicksearch-solr
- This repo will be archived
- When we have solr update: please upate the two following repos:
  - https://git.yale.edu/Library-IT/quicksearch-solr
  steps:
    - in search-frontend directory: 
    - cd qs-solr71-docker
    - update the solr configure in the directory of qs-solr71-docker
    - commit the change
    - create a PR in https://git.yale.edu/Library-IT/quicksearch-solr
  - https://github.com/yalelibrary/yul-solr (Jenkins deploys this repo to servers)
    - change [[the pf or ](https://git.yale.edu/Library-IT/quicksearch-solr/tree/main/common/)](https://git.yale.edu/Library-IT/quicksearch-solr/blob/main/common/fl-defaults.xml) or https://git.yale.edu/Library-IT/quicksearch-solr/blob/main/common/pf-qf-defaults.txt as needed
    - deploy the change in jenkins, Quicksearch/solr   
