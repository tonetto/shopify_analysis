# Shopify app store analysis

Quick & Simple analysis of Shopify's app store (from data scraped and uploaded to [Reddit](https://www.reddit.com/r/datasets/comments/9939fq/shopify_app_marketplace_dataset_2505_apps_253495/) and originally posted at this [link](https://sanjeevan.co.uk/blog/shopify-apps-and-reviews-dataset/)).

## What is it?

A toy jupyter notebook with a few analysis of reviews given to apps found at the Shopify store.

## Is there anything interesting worth my time looking at it?

Nothing was really conclusive, but you can look at it for yourself. Some apps had huge amounts of reviews, that to some extent, looked a bit like bots to me (***cluster 6 in these notebooks***). Maybe I would need to read some related work and see what features are mostly used for bot detection or something similar.

## What was used for these analysis:
To list a few:

  * pandas: for manipulating the data
  * t-sne: non-linear dimensionality reduction
  * powerlaw: a python package for empirical distribution fitting
  * (unsupervised) clustering algorithms [KMeans, GMM]: for clustering apps based on their autocorrelation functions
  * prophet (by Facebook): for timeseries analysis, but so far I used only for timeseries decomposition
  * networkx: for a little bit of network analysis (build based on the shared reviewers between different apps)

## Are you done? Will you continue this anyhow?

Eventually, yes. If I think of anything else interesting to add here.

*Got any questions? Let me know!*

PR's are welcome.
