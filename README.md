# 753PS-proposed-tutchanges
This is an in-progress list of proposed changes to the tutorials for 753PS.

- (Copyediting)
- Code cleanup to conform to tidyverse/google style guide, remove deprecated calls/functions
- Fix bugs like incorrect use of "attr" in frequently-used `get.brokerage` and elsewhere
- Tutorial 1
	- Add discussion of weights implementations in statnet (named) vs igraph (hard-coded)
	- Add discussion of directly accessing statnet `x_stat$gal` components to mirror igraph `is_x` functions
- Tutorial 2
	- Get clarity on igraph and edge weights in path length - not "At this point in time"?
	- Add discussion of `statnet::isolates` as an indicator of igraph `is_connected`
	- Add discussion of unconnected networks and issues presented (esp. wrt upcoming centrality measures), demonstrate with simple constructed example
	- Add code for detecting and self-connecting isolates in both statnet and igraph
- Tutorial 3
	- Mostly code cleanup, content OK
- Tutorial 4
	- Explain differences in eigenvalue values between statnet and igraph; provide code to get them in sync if possible. Get to the bottom of differences in the `airports` networks.
- Tutorial 5
	- Get to the bottom of the vast differences in closeness centrality between the libraries
	- Test and explain Gould-Fernandez
	- Substantiate " it is useful to look at the correlations between scores to understand what they are doing in relation to one another" - why? how?
- Tutorial 6
	- As in all previous tuts, continue to update/build improved nodeinfo dataframe
	- Correct and explain "hamming, correlation, hamming, or gamma" `method`s in `equiv.fun="sedist"`
	- Dendrograms: explain "Node 9 is clearly different compared to the other nodes."
	- Explain why some nodes are not bottom-aligned
	- Explain, don't just show "You may want to experiment with using different methods for the option `equiv.clust(..., cluster.method="")`, replacing the default `cluster.method="complete"` with an alternative such as _single, average_, or _ward.D_. How does changing the clustering method change which nodes are closest to each other?"
	- Explain vacant clusters in dendrograms
	- Investigate/explain why cluster partitions using fixed `h` don't match blockmodel partitions with the same `h` (flomarriage, week 6 hw)
	- "In practice, there are different approaches to identifying the best cutpoint to use as the basis for partitioning, and we explore those in more detail below." - don't see it
	
