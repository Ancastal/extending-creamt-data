# Data layout

| Directory | Purpose |
| --- | --- |
| `inputs/` | Experimental input texts: English source and Italian published reference |
| `machine_translation/` | Unedited LLM machine-translation outputs |
| `postedited_translations/` | Post-edited outputs from the controlled-rotation workflow |
| `annotations/comparative/` | Comparative annotation exports in WebAnno/UIMA XMI format |

`manifest.csv` is the condition-level inventory. It uses paths relative to the repository root.

Condition identifiers intentionally preserve the original study labels. `from_<condition>` identifies a post-edited translation condition derived from that condition; it is not an individual translator identifier.
