# Parallel Bible Corpus (ebible_data)

## Overview

This repository contains a parallel corpus derived from various Bible translations. The primary goal is to provide a resource for machine learning (ML) research and applications, particularly in Natural Language Processing (NLP) and Machine Translation (MT).

The texts have been verse-aligned across different translations to facilitate their use in tasks requiring parallel data.

## Data Source and Licensing

The corpus is compiled from multiple Bible translations all downloaded from eBible.org. These translations are distributed under a variety of licenses, all of which permit sharing and redistribution.

**Important:** Please consult the specific license associated with each translation before using it in your work. Licensing information can typically be found in the `metadata/ebible_status.csv` file.

## Data Creation Process
The scripts, tools, and methodologies used to gather, process, and align the translations in this corpus are maintained within other repositories [ebible_code](https://github.com/davidbaines/ebible_code/) and SIL Global's Language Software Development's [SILNLP](https://github.com/sillsdev/silnlp) repo.

Key metadata files include:
*   `metadata/ebible_status.csv`: Provides status information about the included eBible versions.
*   `metadata/vref.txt`: Contains the standard Bible verse reference system used for alignment.

Intermediate files generated during the process (like raw downloads or project-specific files) are excluded from this repository (see `.gitignore`).

## Hugging Face Dataset

I plan to make this parallel corpus available as a dataset on HuggingFace Hub to promote wider accessibility and easier integration into ML pipelines.

## Repository Structure
```
/
|-- metadata/         # Metadata files (licenses, processing status, verse refs template)
|-- corpus/           # Verse aligned text files for each translation.
```

## Usage

1.  Clone the repository:
    ```bash
    git clone <repository_url>
    cd ebible_data
    ```
