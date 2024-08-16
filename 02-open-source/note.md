Evaluation  Metrics for  Retrieval

=> Hit Rate  - if the retrieved docs is well returned

 MRR (Mean Reciprocal Rank) - how good the ranking is, the more relevant, the  more on top.


Generate Ground Truth Dataset

for each record in FAQ:
    generate 5 questions

for each q in ground truth dataset:
    execute q
    check if doc is in the results