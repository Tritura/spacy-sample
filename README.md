<!-- WEASEL: AUTO-GENERATED DOCS START (do not remove) -->

# 🪐 Weasel Project: Demo pipeline with assembled components

A minimal demo project for spaCy v3 

## 📋 project.yml

The [`project.yml`](project.yml) defines the data assets required by the
project, as well as the available commands and workflows. For details, see the
[Weasel documentation](https://github.com/explosion/weasel).

### ⏯ Commands

The following commands are defined by the project. They
can be executed using [`weasel run [name]`](https://github.com/explosion/weasel/tree/main/docs/cli.md#rocket-run).
Commands are only re-run if their inputs have changed.

| Command | Description |
| --- | --- |
| `download` | Download all required assets and models |
| `convert` | Convert the data to spaCy's binary format |
| `train-ner` | Train the NER model |
| `evaluate-ner` | Evaluate the NER model and export metrics |
| `train-parser` | Train UD_English-EWT |
| `evaluate-parser` | Evaluate on the test data and save the metrics |
| `assemble` | Assemble NER and parser models into one combined pipeline |
| `package` | Package the trained model as a pip package |

### ⏭ Workflows

The following workflows are defined by the project. They
can be executed using [`weasel run [name]`](https://github.com/explosion/weasel/tree/main/docs/cli.md#rocket-run)
and will run the specified commands in order. Commands are only re-run if their
inputs have changed.

| Workflow | Steps |
| --- | --- |
| `all` | `download` &rarr; `convert` &rarr; `train-ner` &rarr; `evaluate-ner` &rarr; `train-parser` &rarr; `evaluate-parser` &rarr; `assemble` &rarr; `package` |

### 🗂 Assets

The following assets are defined by the project. They can
be fetched by running [`weasel assets`](https://github.com/explosion/weasel/tree/main/docs/cli.md#open_file_folder-assets)
in the project directory.

| File | Source | Description |
| --- | --- | --- |
| [`assets/ner/train.json`](assets/ner/train.json) | Local | Demo NER training data |
| [`assets/ner/dev.json`](assets/ner/dev.json) | Local | Demo development data |
| `assets/parser/UD_English-EWT` | Git |  |

<!-- WEASEL: AUTO-GENERATED DOCS END (do not remove) -->
