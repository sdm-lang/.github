## Simple Domain Modeling Language (SDML)

![SDML Logo Text](https://raw.githubusercontent.com/sdm-lang/.github/main/profile/horizontal-text.svg)

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

## Source Editor

The following table demonstrates the current editor support for SDML. Note that the tree-sitter parser and TextMate
grammar alone provides multiple editor support while the Sublime Text grammar also covers the `bat` command-line tool.

| Repo                                                  | Tool                                         | Highlighting                     | Snippets                                     | Indentation | Folding | Linting             | CLI                         |
|-------------------------------------------------------|----------------------------------------------|----------------------------------|----------------------------------------------|-------------|---------|---------------------|-----------------------------|
| [here](https://github.com/sdm-lang/emacs-sdml-mode)   | [Emacs](https://www.gnu.org/software/emacs/) | Complete, using Tree-Sitter      | Extensive, using `abbrev-mode` and skeletons | Yes         | Yes     | Yes, using flycheck | Yes, including in org-mode. |
| [here](https://github.com/sdm-lang/sdml-vscode)      | [VSCode](https://code.visualstudio.com/)     | Yes, using TextMate grammar      | Yes, converted from TextMate                 | Simple      | No      | No                  | Partial                     |
| [here](https://github.com/sdm-lang/SDML.tmbundle)     | [TextMate](https://macromates.com/)          | Yes, a `.tmLanguage` grammar     | Yes, extensive                               | Simple      | No      | No                  | Partial                     |
| [here](https://github.com/sdm-lang/sdml-sublime-text) | [Sublime Text](https://www.sublimetext.com/) | Yes, a `.sublime-syntax` grammar | No                                           | No          | No      | No                  | No                          |
| in Sublime                                            | [bat](https://github.com/sharkdp/bat)        | Yes, using Sublime Text grammar  | N/A                                           | N/A          | N/A      | N/A                  | N/A                          |
| in TextMate                                           | Jet Brains                                   | Yes, using TextMate Bundle       | Yes                                          | No          | No      | No                  | No                          |
|                                                       | Neovim                                       | Using Tree-Sitter                | ?                                            | ?           | ?       | ?                   | ?                           |

Instructions exist for integrating tree-sitter parsers into Neovim, this is not tested.

## Other Tools

* `highlightjs-sdml` -- Syntax highlighting of SDML source files in HTML resources.

## Licenses

All repositories are dual licensed with [Apache-2.0](https://opensource.org/license/apache-2-0)
and [MIT](https://opensource.org/license/mit) unless otherwise stated.

### Contributions

Unless you explicitly state otherwise, any contribution intentionally submitted
for inclusion in the work by you, as defined in the Apache-2.0 license, shall
be dual licensed as above, without any additional terms or conditions.

For information on contributing to this project, see the following:

1. Project [Contribution Guidelines](./CONTRIBUTING.md)
1. Project [Code of Conduct](./CODE_OF_CONDUCT.md).
