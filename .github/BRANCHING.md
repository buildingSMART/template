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

Git diagram
```
---
title: Example Git diagram
---
gitGraph
   commit
   commit
   branch develop
   checkout develop
   commit
   commit
   checkout main
   merge develop
   commit
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