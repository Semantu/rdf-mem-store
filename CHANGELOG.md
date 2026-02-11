# @\_linked/rdf-mem-store

## 1.0.1

### Patch Changes

- [#15](https://github.com/Semantu/rdf-mem-store/pull/15) [`496f803`](https://github.com/Semantu/rdf-mem-store/commit/496f80371914faab20cd098129c039015d8ce170) Thanks [@flyon](https://github.com/flyon)! - update core dependency

## 1.0.0

### Major Changes

Initial extraction from the LINCD monolith. Moves all RDF model classes, the in-memory quad store, and the query resolver into a standalone package.

- RDF models (NamedNode, Literal, BlankNode, Quad, Graph) and all RDF collections extracted from lincd.
- InMemoryStore implements IQuadStore from @\_linked/core.
- LocalQueryResolver resolves core’s query objects against the in-memory quad graph.
- toNamedNode helper bridges core’s NodeReferenceValue ({id: string}) to NamedNode instances.
