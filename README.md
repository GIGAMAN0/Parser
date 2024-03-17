# Noun Phrase Parsing with Context-Free Grammar

This project involves developing an AI system to parse sentences and extract noun phrases using context-free grammar rules.

## Introduction

Parsing sentences and extracting noun phrases are essential tasks in natural language processing. Understanding the structure of sentences helps computers comprehend their meaning and extract relevant information. In this project, we utilize context-free grammar to parse English sentences and identify noun phrases.

## Files

- `parser.py`: Contains the implementation of functions to preprocess sentences, define context-free grammar rules, parse sentences, and extract noun phrases.
- `README.md`: Documentation of the project, including instructions, background, and implementation details.
- `sentences/`: Directory containing text files, each containing an English sentence.

## Usage

1. Download the distribution code from the provided link and unzip it.
2. Navigate to the parser directory.
3. Run the command `pip3 install -r requirements.txt` to install the required dependency (nltk).
4. Execute the command `python parser.py` to parse sentences and extract noun phrases.

## Background

The project involves implementing a parser using context-free grammar rules to parse English sentences. Each sentence is preprocessed and parsed according to the defined grammar rules. Noun phrases are extracted from the parsed trees using specified criteria.

## Implementation Details

- **Preprocess**: The preprocess function tokenizes and lowercases input sentences, returning a list of words excluding non-alphabetic characters.
- **Context-Free Grammar Rules**: The NONTERMINALS variable defines context-free grammar rules for generating nonterminal symbols. Each rule specifies how symbols can be rewritten, incorporating noun phrases (NP) to represent subjects of sentences.
- **Parsing and Noun Phrase Extraction**: The main function parses input sentences according to the defined grammar rules, generating parse trees. Noun phrase chunks are extracted from the parse trees using the np_chunk function.

## Observations

- Designing effective context-free grammar rules is crucial for accurate sentence parsing.
- The balance between over-generation and under-generation of sentences should be maintained to ensure the parser's effectiveness.
- English grammar ambiguity can lead to multiple parse trees for a single sentence, requiring careful consideration during noun phrase extraction.

