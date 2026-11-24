# files-to-prompt

Turns a set of files and folders into one text document for an LLM.

## Language

**Output**:
The single text document files-to-prompt produces from the chosen files, written to stdout or to the `-o` file.
_Avoid_: Prompt (ambiguous with the user's own question to the LLM), dump

**Notebook clearing**:
Removing a Jupyter notebook's run results and bulky non-content parts from the copy that goes into the **Output**, keeping it a valid notebook. The notebook file itself is never changed.
_Avoid_: Notebook stripping, cleaning

**Selection**:
The files and folders a user ticks in the TUI for one run. A ticked folder includes everything inside it except entries unticked individually. It is not remembered between runs.
_Avoid_: Include list, allowlist
