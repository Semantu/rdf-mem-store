# @\_linked/rdf-mem-store

## 1.0.0

### Major Changes
Initial extraction from the LINCD monolith. Moves all RDF model classes, the in-memory quad store, and the query resolver into a standalone package.
- RDF models (NamedNode, Literal, BlankNode, Quad, Graph) and all RDF collections extracted from lincd.
- InMemoryStore implements IQuadStore from @_linked/core.
- LocalQueryResolver resolves core’s query objects against the in-memory quad graph.
- toNamedNode helper bridges core’s NodeReferenceValue ({id: string}) to NamedNode instances.
