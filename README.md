# DKFZ_short_example
Explore associations between genes and diseases

I wrote a small analysis script that queries the Open Targets REST API to explore associations between genes and diseases. The script supports two modes: “gene → all associated diseases” and “disease → all associated targets.” For each query, it parses the JSON response, prints a clean association table with overall confidence scores, and computes summary statistics like mean and standard deviation. All results are also logged to disk, so the output can be reviewed, shared, or audited later without rerunning the query.
