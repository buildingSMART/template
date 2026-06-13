# Git branching policy

```
main
├── release/4.3
│   ├── feature/4.3-bugfix-a
│   └── hotfix/4.3.2
└── release/4.4
    ├── feature/new-capability
    ├── feature/api-update
    └── hotfix/4.4.1
```

<!-- Guide how to use Mermaid GitGraph: https://mermaid.js.org/syntax/gitgraph.html. -->
```mermaid
---
title: Branching policy
---
gitGraph
   commit development
   commit development
   branch ver/1.0.x
   checkout ver/1.0.x
   commit
   branch bugfix/561-docs-typo
   merge ver/1.0.x
   commit
   checkout development
   branch ver/1.1.x 
   commit tag: "1.1.0"
   commit
   commit tag: "1.1.1"
   branch ver/2.0.x
   branch feature/421-partOf
   branch feature/123-grouping
   checkout development
   commit id: "1" tag: "1.1.0_vote"
   commit
```
	
diagram
```mermaid
sequenceDiagram
   To Do->>+Draft: Pixar initial review
   To Do->>+Draft: Community review
   Draft-->>+Hold: Core proposal needs more iteration
   Hold-->>-Draft: Pixar core concerns addressed
   Draft->>+Finalizing: Pixar & community comments addressed
   Finalizing->>+Published: Final cleanup
   Published->>+Implemented: Implementation in OpenUSD
   To Do-->>+Hold: Core proposal needs more iteration
   To Do-->>+Closed: Proposal retracted
   Draft-->>+Closed: Proposal retracted
   Hold-->>+Closed: Proposal retracted
   Finalizing-->>+Closed: Proposal retracted
```

```mermaid
sequenceDiagram
   To Do->>+Draft: Pixar initial review
   To Do->>+Draft: Community review
   Draft-->>+Hold: Core proposal needs more iteration
   Hold-->>-Draft: Pixar core concerns addressed
   Draft->>+Finalizing: Pixar & community comments addressed
   Finalizing->>+Published: Final cleanup
   Published->>+Implemented: Implementation in OpenUSD
   To Do-->>+Hold: Core proposal needs more iteration
   To Do-->>+Closed: Proposal retracted
   Draft-->>+Closed: Proposal retracted
   Hold-->>+Closed: Proposal retracted
   Finalizing-->>+Closed: Proposal retracted
```


python
```Python
import test

a = 2.0

print(a)

```



stl
```stl
solid cube_corner
  facet normal 0.0 -1.0 0.0
    outer loop
      vertex 0.0 0.0 0.0
      vertex 1.0 0.0 0.0
      vertex 0.0 0.0 1.0
    endloop
  endfacet
  facet normal 0.0 0.0 -1.0
    outer loop
      vertex 0.0 0.0 0.0
      vertex 0.0 1.0 0.0
      vertex 1.0 0.0 0.0
    endloop
  endfacet
  facet normal -1.0 0.0 0.0
    outer loop
      vertex 0.0 0.0 0.0
      vertex 0.0 0.0 1.0
      vertex 0.0 1.0 0.0
    endloop
  endfacet
  facet normal 0.577 0.577 0.577
    outer loop
      vertex 1.0 0.0 0.0
      vertex 0.0 1.0 0.0
      vertex 0.0 0.0 1.0
    endloop
  endfacet
endsolid
```


geojson
```geojson
{
  "type": "FeatureCollection",
  "features": [
    {
      "type": "Feature",
      "id": 1,
      "properties": {
        "ID": 0
      },
      "geometry": {
        "type": "Polygon",
        "coordinates": [
          [
              [-90,35],
              [-90,30],
              [-85,30],
              [-85,35],
              [-90,35]
          ]
        ]
      }
    }
  ]
}
```