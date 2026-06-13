# Git branching policy

### What is this?


## Principles

The main working branch is the development, which displays the state of the most current standard proposal being developed. Version branches are to be found on branches starting with ver for example ver/1.1.x. The official versions of the standard are marked with tags, for example 1.0.0, and can be also found in GitHub realeses.

main = future
version branches = maintained release lines
tags = exact released artifacts


<!-- Guide how to use Mermaid GitGraph: https://mermaid.js.org/syntax/gitgraph.html. -->
```mermaid
---
title: Branching policy
config:
  theme: 'base'
---
gitGraph
   commit id: "001"
   commit id: "002"
   branch ver/1.0.x
   checkout ver/1.0.x
   commit id: "003"
   commit id: "004" tag: "1.0.0"
   branch bugfix/561-docs-typo
   checkout bugfix/561-docs-typo
   commit id: "005"
   checkout ver/1.0.x
   merge bugfix/561-docs-typo
   commit id: "006"
   checkout main
   branch ver/1.1.x 
   checkout ver/1.1.x 
   commit id: "007"
   commit id: "008" tag: "1.1.0"
   commit id: "009"
   commit id: "010" tag: "1.1.1"
   checkout main
   branch feature/421-partOf
   checkout feature/421-partOf
   commit id: "011"
   checkout main
   branch feature/123-grouping
   checkout feature/123-grouping
   commit id: "012"
   checkout main   
   commit id: "013"
```
<!-- cherry-pick id:"08" parent:"12" -->
<!-- merge main id:"MERGE" -->
	
## Naming convention

**Commit name** should be...
**Branch name** should be...
**Tag name** should be...

	