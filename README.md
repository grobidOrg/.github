# GROBID Organization

## About GROBID

GROBID (GeneRation Of BIbliographic Data) is a machine learning library for extracting, parsing and re-structuring raw documents such as PDF into structured XML/TEI encoded documents with a particular focus on technical and scientific publications.

## The Organization

GROBID is an **open source project** supported by:
- **[INRIA](https://www.inria.fr/)** (French National Institute for Research in Digital Science and Technology)
- **MESRE** (French Ministry of Higher Education, Research and Innovation)

The project is **maintained by [Luca Foppiano](https://github.com/lfoppiano)**, continuing the work initiated by [Patrice Lopez](https://github.com/kermitt2), GROBID's original creator.

## History

GROBID was created in 2008 by Patrice Lopez as a personal project, following a suggestion by Laurent Romary (Inria, France). In 2011, the tool was made available as open source. Since the beginning, development has been continuous, facilitated in particular by the ongoing support of Inria.

## Key Functionalities

GROBID offers the following functionalities for extracting and structuring scientific documents:

- **Metadata extraction and parsing**: title, abstract, authors, affiliations, keywords
- **Reference extraction and parsing**: with approximately 0.87 F1-score (Deep Learning)
- **Citation context recognition** and resolution of full bibliographical references
- **Full text extraction and structuring**: paragraphs, section titles, reference callouts, figures, tables
- **PDF coordinates** to create "augmented" interactive PDFs
- **Parsing of references in isolation**: over 0.90 F1-score at instance level
- **Name parsing**: author names, affiliations, addresses
- **Consolidation/resolution** of bibliographical references via biblio-glutton or CrossRef API
- **Funding information extraction** with optional matching with CrossRef Funder Registry
- **Copyright and license identification** associated with the document

## Production Deployments

GROBID is used in production by numerous major organizations and platforms:
- OpenAlex
- ResearchGate
- Semantic Scholar
- HAL Research Archive
- scite.ai
- Matilda
- Academia.edu
- Internet Archive Scholar
- INIST-CNRS
- CERN (Invenio)
- And many more...

## Repositories and Resources

### Main Repository
- **[grobid](https://github.com/kermitt2/grobid)**: Main GROBID library

### Clients
- **[grobid-client-python](https://github.com/kermitt2/grobid-client-python)**: Python client for GROBID
- **[grobid-client-java](https://github.com/kermitt2/grobid-client-java)**: Java client for GROBID
- **[grobid-client-node](https://github.com/kermitt2/grobid-client-node)**: Node.js client for GROBID

### Specialized Modules
- **[software-mention](https://github.com/ourresearch/software-mentions)**: Recognition of software mentions
- **[datastet](https://github.com/kermitt2/datastet)**: Identification of datasets in scientific articles
- **[grobid-quantities](https://github.com/kermitt2/grobid-quantities)**: Recognition and normalization of physical quantities
- **[grobid-superconductors](https://github.com/lfoppiano/grobid-superconductors)**: Recognition of superconductor materials
- **[entity-fishing](https://github.com/kermitt2/entity-fishing)**: Wikidata entity extraction
- **[grobid-ner](https://github.com/kermitt2/grobid-ner)**: Named entity recognition
- **[grobid-astro](https://github.com/kermitt2/grobid-astro)**: Recognition of astronomical entities
- **[grobid-dictionaries](https://github.com/MedKhem/grobid-dictionaries)**: Dictionary structuring

### Tools and Utilities
- **[delft](https://github.com/kermitt2/delft)**: Deep Learning framework for sequence labeling
- **[biblio-glutton](https://github.com/kermitt2/biblio-glutton)**: Bibliographic consolidation service
- **[pdfalto](https://github.com/kermitt2/pdfalto)**: Extraction of visual/layout information from PDFs
- **[article-dataset-builder](https://github.com/kermitt2/article-dataset-builder)**: Creation of structured scientific article corpora

## Documentation

📚 **Full documentation**: [https://grobid.readthedocs.io](https://grobid.readthedocs.io)

The documentation covers:
- Quick start guide
- Installation and configuration
- API and web services
- Model training
- Benchmarking and evaluation
- Docker deployment

## Demo

### Demo Servers

Two public demo servers are available thanks to HuggingFace:

- **With Deep Learning + CRF models**: [https://kermitt2-grobid.hf.space/](https://kermitt2-grobid.hf.space/)
- **With CRF only (faster)**: [https://kermitt2-grobid-crf.hf.space/](https://kermitt2-grobid-crf.hf.space/)

⚠️ **Warning**: These demo servers have quota limitations. For serious use, please deploy your own GROBID server.

## Performance

GROBID is designed for speed and high scalability:

- **Large-scale processing**: Approximately 10.6 PDF per second (915,000 PDF per day)
- **Production ready**: Used by numerous platforms in production
- **Parallelization**: Native support for parallel processing

## License

GROBID is distributed under [Apache 2.0](http://www.apache.org/licenses/LICENSE-2.0) license.

The documentation is distributed under [CC-0](https://creativecommons.org/publicdomain/zero/1.0/) license and annotated data under [CC-BY](https://creativecommons.org/licenses/by/4.0/) license.

## Contact

- **Main Maintainer**: Luca Foppiano ([GitHub](https://github.com/lfoppiano))
- **Original Creator**: Patrice Lopez ([patrice.lopez@science-miner.com](mailto:patrice.lopez@science-miner.com))

## How to Cite GROBID

If you use GROBID in your research, please cite:

```bibtex
@misc{GROBID,
    title = {GROBID},
    howpublished = {\url{https://github.com/kermitt2/grobid}},
    publisher = {GitHub},
    year = {2008--2025},
    archivePrefix = {swh},
    eprint = {1:dir:dab86b296e3c3216e2241968f0d63b68e8209d3c}
}
```

## Contributing

Contributions are welcome! If you contribute to GROBID, you agree to share your contribution under the licenses mentioned above.

For more information on contributing to the project, consult the documentation on GitHub.

---

*GROBID is an open source project supported by INRIA and MESRE, maintained by Luca Foppiano in continuation of the work of Patrice Lopez.*
