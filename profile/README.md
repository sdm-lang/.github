## Simple Domain Modeling Language (SDML).

```
        ___          _____          ___
       /  /\        /  /::\        /__/\
      /  /:/_      /  /:/\:\      |  |::\
     /  /:/ /\    /  /:/  \:\     |  |:|:\    ___     ___
    /  /:/ /::\  /__/:/ \__\:|  __|__|:|\:\  /__/\   /  /\
   /__/:/ /:/\:\ \  \:\ /  /:/ /__/::::| \:\ \  \:\ /  /:/
   \  \:\/:/~/:/  \  \:\  /:/  \  \:\~~\__\/  \  \:\  /:/
    \  \::/ /:/    \  \:\/:/    \  \:\         \  \:\/:/
     \__\/ /:/      \  \::/      \  \:\         \  \::/
       /__/:/        \__\/        \  \:\         \__\/
       \__\/          Domain       \__\/          Language
        Simple                      Modeling
```

The Simple Domain Modeling Language (SDML) is a small data-oriented language for constructing, documenting, and
reasoning about a conceptual domain model. At it's core SDML comprises:

1. a *semantic model* whose structure and semantics are described in RDF with an OWL ontology,
2. a *surface syntax* for editing and sharing model artifacts, and
3. a *constraint language* to capture model invariants not covered by the data descriptions in the surface syntax.

For more information on the language, see the [documentation](https://sdml.io/).

The core repositories are:

* `tree-sitter-sdml` -- The tree-sitter implementation of the SDML language. Note that the grammar defined in this
  repository is the definitive specification.
* `rust-sdml` -- Parser and Generator libraries and a CLI for manipulating SDML source files.
* `sdml.io` -- The documentation for the SDML language, available at [https://sdml.io](https://sdml.io).

Additional support for language presentation and editing is provided via:

* `emacs-sdml-mode` -- An [Emacs](https://www.gnu.org/software/emacs/) package for syntax highlighting, indenting, and linting for SDML source files.
* `SDML.tmbundle` -- A [TextMate](https://macromates.com/) language bundle for syntax highlighting and snippet support.
* `emacs-vscode` -- A [VSCode](https://code.visualstudio.com/) extension for syntax highlighting and snippet support.
* `highlightjs-sdml` -- Syntax highlighting of SDML source files in HTML resources.
