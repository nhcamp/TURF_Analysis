# TURF_Analysis

This code implements a simple, non-optimal, TURF analysis in Python. Given a set of features, here reasons, and the most popular option,
this code will enumerate through sets of unique identifiers to build a list of incremental feature addidtions and calculate the cumulative
reach of each additional feature. 

This simple tool wasn't available elsewhere online so I put this together quickly for work use.

It's important to note that this TURF is sub-optimal in a large and complex feature space. Because it evaluates each combination of features starting with the single largest reach, it will not account for situations where the feature of largest individual reach is NOT included in the mix. This doesn't happen in practice but is theoretically possible. In 99.9% of non-theoretical use cases, this method will give you the results you need.
