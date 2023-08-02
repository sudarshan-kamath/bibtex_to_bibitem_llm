# BibTeX to Bibitem Converter with ChatGPT Integration

This repository contains a Python script that converts BibTeX entries from a `.bib` file into formatted Bibitem references. It utilizes the ChatGPT model to interactively assist in generating Bibitem references based on the provided BibTeX entries.

## Requirements

- Python (>=3.6)
- `dotenv`
- `bibtexparser`
- `langchain` (ChatOpenAI and schema modules)

## Installation

1. Clone this repository:

```bash
git clone https://github.com/sudarshan-kamath/bibtex_to_bibitem_llm.git
cd bibtex_to_bibitem_llm
```

2. Install the required dependencies:

```bash
pip install -r requirements.txt
```

3. Obtain OpenAI API Key

   To use the ChatGPT model, you'll need an API key from OpenAI. You can follow their instructions to obtain an API key and set up your environment variables.

## Usage

1. Create a `.env` file in the project directory and add your OpenAI API key:

```
OPENAI_API_KEY=your-api-key
```

2. Prepare your BibTeX file (`sources.bib`) with the BibTeX entries you want to convert.

3. Customize the `prompt.txt` file with the initial prompt you want to use for generating each Bibitem reference.

4. Run the conversion script:

```bash
python convert_bib_to_bibitem.py
```

The script will read the BibTeX entries from `sources.bib`, generate corresponding Bibitem references using ChatGPT, and write the results to an `output.txt` file.

## Customization

- You can adjust the `max_tokens` and `temperature` parameters in the `ChatOpenAI` initialization to control the length and creativity of the generated responses.
- Modify the `prompt.txt` file to change the initial prompt presented to the ChatGPT model for each entry.

## Acknowledgments

The ChatGPT model provided by OpenAI powers the interactive conversion process in this tool.

---

*Note: This README provides a general overview of the BibTeX to Bibitem Converter with ChatGPT Integration. Make sure to adapt the instructions and explanations to match your actual file structure and use case.*