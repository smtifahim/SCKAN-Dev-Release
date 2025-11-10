# SCKAN-Dev-Release
This repository is created to publish the developmental releases of the SCKAN ontology for **rapid testing and validation**. Each release will include the major artifacts relevant to the core SCKAN ontology generated through the documented, reproducible process, including post-processed, reasoned, and merged ontologies, a Blazegraph journal, and full provenance records.

## Artifacts

- `npo-sckan-merged.ttl`: Merged SCKAN/NPO ontology (pre-reasoning)
- `npo-sckan-merged-reasoned.ttl`: Fully reasoned SCKAN/NPO ontology (ELK/ROBOT)
- `chebi.ttl`, `uberon.ttl`, `uberon-reasoned.ttl`, `taxslim.ttl`, `sparc-community-terms.ttl`: Key imported ontologies
- `sckan-partial-order-rdfstar.ttl`: SCKAN neural circuit model (RDF-star)
- `blazegraph.jnl`: Blazegraph triple store journal (loadable for SPARQL queries)
- `prov-record.ttl`: Provenance record for the build process
- `prefixes.conf`: Prefix configuration for downstream tools

## Reproducibility

All steps to generate these artifacts are documented and selectively follow the SCKAN release workflow:
- Ontology build and post-processing (pyontutils/neurondm)
- Merging and reasoning (ROBOT/ELK)
- Custom serialization (ttlser)
- Blazegraph journal generation
- Provenance record creation

## Notes

- This is a developmental release for testing and validation. Artifacts and processes may change in future releases.
- For full details and step-by-step instructions, see the `SCKAN-Release-Process`.
- For questions or reproducibility issues, please open an issue or contact the maintainers.
