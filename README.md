# Search Engine — TF-IDF & BM25

A search engine in **Java** that indexes a text corpus and ranks documents against user queries using the **TF-IDF** and **BM25** relevance models. It includes a full text-processing pipeline and robust error handling.

## Features

- **Text preprocessing** — lowercasing, **Porter stemming** (Snowball), and stop-word removal
- **Two ranking models** — TF-IDF and BM25, for comparison
- **Vocabulary & document modeling** — core classes for documents, words, and the corpus
- **Query evaluation** — relevance scoring across the corpus
- **Exception handling** for corpus and query errors

## Tech Stack

- Java
- Snowball / Porter stemmer (`snowball-stemmer-1.3.0.581.1.jar`)

## Build & Run

```bash
git clone https://github.com/ZinebMEFTAH/Search-Engine.git
cd Search-Engine
# Compile (with the stemmer on the classpath)
javac -cp "snowball-stemmer-1.3.0.581.1.jar" -d bin src/**/*.java
# Run
java -cp "bin:snowball-stemmer-1.3.0.581.1.jar" Main
```

## Corpus & Resources

- `BOOK.txt`, `WIKIPEDIA.txt` — sample document corpora
- `stopList.txt` — stop words

## Architecture

- **Model** — `Document`, `Word`, `Vocabulary`, and related classes
- **Engine** — preprocessing, indexing, and TF-IDF / BM25 scoring

## Team

Meftah Zineb · Medjber Syphax

## Notes

Information-retrieval project implementing the core ranking models behind modern search from scratch.
