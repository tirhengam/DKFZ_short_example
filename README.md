# DKFZ_short_example


This script queries the Open Targets REST API to explore associations between genes and diseases. The script supports two modes: 
“gene → all associated diseases” and “disease → all associated targets.” 

For each query, it parses the JSON response, prints a clean association table with overall confidence scores
Technical Stack
Language: Python 3.8+
API: Open Targets Platform REST API
Key Library: opentargets - Official Python client
Usage Examples
Original Version
bash
# Query by target (gene)
python original/query_target.py -t ENSG00000197386

# Query by disease
python original/query_target.py -d EFO_0000249
Sample Output 
Diseases associated with target: ENSG00000197386 

 Index    |          Target-Disease              |   Overall Score
-------------------------------------------------------------------------
     0    | ENSG00000197386-EFO_0000249          |           0.847
     1    | ENSG00000197386-EFO_0003767          |           0.623
     2    | ENSG00000197386-EFO_0000305          |           0.501

Total associations: 3
A command-line tool for querying gene-disease associations using the Open Targets Platform REST API. Demonstrates API integration and practical bioinformatics application.
