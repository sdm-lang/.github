## Simple Domain Modeling Language (SDML).

The Simple Domain Modeling Language (SDML) is a small data-oriented language for constructing, documenting, and
reasoning about a conceptual domain model. At it's
core SDML comprises:

1. a *semantic model* whose structure and semantics are described in RDF by an OWL ontology
2. a *surface syntax* for editing and sharing model artifacts
3. a *constraint language* to capture model invariants not covered by the data descriptions in the surface syntax.

For more information on the language, see the [documentation](https://sdml.io/).

The core repositories are:

- `tree-sitter-sdml` -- The tree-sitter implementation of the SDML language. Note that the grammar defined in this
  repository is the definitive specification.
* `sdml.io` -- The documentation for the SDML language, available at [https://sdml.io](https://sdml.io).
* `rust-sdml` -- Parser and Generator libraries and a CLI for manipulating SDML source files.
* `emacs-sdml-mode` -- Syntax highlighting, indenting, and linting for SDML source files.
