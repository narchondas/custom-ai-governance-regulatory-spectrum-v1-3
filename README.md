## Overview

This repository contains a reusable Google Colab notebook that allows researchers to apply the AI Governance Regulatory Spectrum Artefact v1.3 to their own documents.

Unlike the replication artefact, which reproduces a fixed thesis corpus, this custom version is designed for new user-selected documents.

Researchers can upload AI-related legal, policy, strategic, institutional or organisational PDF documents and analyse where they are positioned on a two-dimensional regulatory spectrum.

## What the notebook does

The notebook maps documents across two axes:

- **X-axis:** rights- and citizen-oriented safeguards ↔ innovation
- **Y-axis:** voluntary/soft-law ↔ mandatory/control

The same v1.3 logic is applied:

- no word-level weights;
- all terms and phrases count as one occurrence;
- the document-level legal-force multiplier is applied only to the mandatory/control count;
- the same four analytical vocabularies are used;
- the same scoring equations and visual outputs are generated.

## How to use the custom notebook

1. Open the notebook in Google Colab.
2. Upload the PDF documents you want to analyse.
3. Run the file-check cell to confirm the exact filenames.
4. Edit the metadata table by replacing:
   - `DOC_01`, `DOC_02`;
   - `your_document_1.pdf`, `your_document_2.pdf`;
   - `Group I`, `Group II`;
   - document titles, years, institutions and document types.
5. Assign the appropriate legal-force multiplier.
6. Run all cells in order.
7. Download the generated Excel and HTML outputs.

## Suggested legal-force multipliers

| Document type | Multiplier |
|---|---:|
| Binding legislation / regulation | 1.50 |
| Executive order | 1.20 |
| Legislative proposal / bill not in force | 1.10 |
| Policy communication / strategy | 0.80 |
| Framework / guidance | 0.70 |
| Voluntary pact / code | 0.60 |

## Outputs generated

The custom notebook can generate:

- regulatory spectrum scatter plot;
- four-component vocabulary profile;
- heatmap of component intensity;
- quadrant distribution chart;
- top driver terms by document group;
- slope chart comparing safeguards and innovation;
- document-type comparison chart;
- analytical vocabulary audit tables;
- exported Excel and HTML outputs.

## Open in Google Colab

[![Open Custom Test Notebook in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/narchondas/custom-ai-governance-regulatory-spectrum-v1-3/blob/main/notebooks/AI_Governance_Regulatory_Spectrum_Artefact_v1_3_Custom_Test.ipynb)

## Limitations

The artefact is dictionary-based and should be interpreted as a diagnostic mapping tool rather than a definitive legal or policy assessment.

Results depend on the quality of PDF extraction, the metadata supplied by the researcher, the selected document groups, the assigned legal-force multipliers, the predefined vocabularies, and the length and structure of the uploaded documents.

Researchers should inspect the vocabulary audit table before drawing substantive conclusions.
