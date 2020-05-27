![status](https://img.shields.io/badge/Code%20License-Apache%202.0-yellow.svg)
![status](https://img.shields.io/badge/Text%20License-CC%20BY%204.0-yellow.svg)

# This Repository
There is a complete description of the process to be found in `/template/HOW-TO-SPEC.md`. You should keep that document for others to understand how to contribute.

![graph](/template/images/7P-Lifecycle.drawio.svg)

## Process
This repo contains a template for your specifications. Copy the `template` folder to your project repository and rename it to `specifications`. It is absolutely essential that the specs "live" in the same repository as the code, because changes to the code necessitate changes to the specification - and vice versa.

This process described below shows the evolution of the specifications describing a project as it evolves from an idea to a stable implementation.

- `1 - SCOPE`: Create a proposal and get stakeholder signoff.
- `2 - RFP`: Write a request for proposals (RFP) and answer that request with scoped Proposals to Requests (PTR).
- `3 - SPECS`: Write specifications for engineering and requirements.
- `4 - RFC`: Use the RFC process to modify decisions already made.
- `5 - BOM`: Maintain a list of dependencies.

## Tools

### drawio
We recommend installing the [drawio extension for VS Code](https://github.com/hediet/vscode-drawio.git). It allows you to edit the diagrams in VS Code, and export them to your repository. Maintaining versions inline with the current state of the specifications. For now, consider using the insiders build version of this, because then if you save the diagram as `file.drawio.svg` you can edit it with the plugin & display it in your markdown documents.

### mdbook
> Todo: Finalize gh action for creating a mdbook and publishing it. [This workflow from Bee](https://github.com/iotaledger/bee-rfcs/blob/master/.github/workflows/gh-rfcs-mdbook.yml) is a good start, but needs adaptation to 7PEC. It requires a `gh-pages`  branch and there has to be a deployment key on the repo admin panel.

### Bill of Materials
It is fundamentally essential that a software bill of materials is maintained for every project. This is important from not only a security standpoint, but also from a license compliance standpoint. Many programming languages offer automated systems for this, and automation is important for guaranteeing that the software product's BOM stays inline with the current state of the project.

> Todo: Create a github action that watches files where versions of software are declared / imported and rerun automation.

## Licensing
(c) 2020 Iota Stiftung

- All code in this library is licensed according to [Apache 2.0](https://www.apache.org/licenses/LICENSE-2.0.html).
- All text in this library is licensed according to [Creative Commons Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/).
