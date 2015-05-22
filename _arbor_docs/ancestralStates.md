---
layout: post
title: aceArbor
author: Arbor core team
---

## aceArbor: function

### Arbor collection
phylogenies

### Description
Estimates ancestral states for either discrete or continuous variables using
various methods.

### Usage

### Arguments
- table: A data table including species names
- tree: A phylogenetic tree
- column: The name of the column to analyze
- type: The character type
  - discrete: a character with a discrete number of states}
  - continuous: a continuously varying character}
  - fromData: will attempt to determine the data type from the data itself
- method: specifies the method used to reconstruct ancestral character states
  - marginal: marginal ancestral state reconstructions, which reconstruct each node integrating over all possibilities at all other nodes in the tree; this is typically the method used in the literature to reconstruce ACEs}
  - joint: joint ancestral reconstructions, which give the configuration of ancestral states that together maximize the likelihood of the data given model parameters}
  - mcmc: reconstruct ancestral states using Bayesian MCMC. Note that the discrete version of this doesn't seem to work, and even if it did work it is not a full MCMC ancestral state method}
  - stochastic: create stochastic character map}

###Outputs
Function outputs a table and a plot with results of the ancestral state reconstruction.

### See also

### Examples