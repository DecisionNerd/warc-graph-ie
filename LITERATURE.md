# Literature Review: Web Archive Information Extraction for Knowledge Graphs

## Introduction

Web archives, particularly in WARC format, have become increasingly important for preserving and analyzing web content. This review focuses on the intersection of web archiving and knowledge graph construction, specifically examining approaches for extracting structured information from WARC/WET files. The emergence of Large Language Models (LLMs) has introduced new possibilities for enhancing knowledge extraction from web archives.

[1] Vaughan, T. (2024). "Web Archiving File Formats Explained", Common Crawl Blog

## WARC Format Overview

The WARC (Web ARChive) format is an ISO standard (ISO 28500:2017) that provides a method for combining multiple digital resources into an aggregate archive file. As the industry standard for web archiving, it offers several key advantages over its predecessor, the ARC format:

- Support for storing web crawls as sequences of content blocks
- Enhanced metadata storage capabilities
- Storage of request and response headers
- Support for new record types like resource revisit, metadata, and conversion
- Better scalability and standardization
- HTTP/1.0-like stream structure with headers and CRLF delimiters

[2] ISO 28500:2017 - Information and documentation -- WARC file format

## Information Extraction from Web Archives

### 1. Text Extraction from WET Files

WET (WARC Encapsulated Text) files are specialized text-only extracts from WARC files, containing the plain text content of web pages. This format is particularly useful for information extraction because:

- Contains only the body text of web pages, excluding HTML code, images, and media
- Removes HTML markup and formatting
- Preserves the essential textual content
- Reduces processing overhead compared to full WARC files
- Enables more efficient text analysis and entity extraction
- Ideal for linguistic analysis and content categorization

[3] Vaughan, T. (2024). "Web Archiving File Formats Explained", Common Crawl Blog

### 2. Knowledge Graph Construction Approaches

Several approaches have been developed for building knowledge graphs from web archive content:

#### a) Entity Extraction and Relation Mining

- Named Entity Recognition (NER) on extracted text
- Relation extraction between identified entities
- Temporal information extraction for temporal knowledge graphs
- Domain-specific entity and relation patterns

[4] Nguyen, D. Q., et al. (2020). "A Survey of Embedding Models for Knowledge Graph Completion"

#### b) Graph Construction Methods

- Entity-centric graph construction
- Event-based knowledge graph creation
- Temporal knowledge graph development
- Multi-modal knowledge graph integration

[5] Wang, Q., et al. (2021). "Knowledge Graph Construction: A Comprehensive Survey"

### 3. Challenges and Solutions

Key challenges in web archive information extraction include:

- Handling different languages and character encodings
- Dealing with duplicate content
- Managing temporal aspects of web content
- Processing large-scale web archives efficiently
- Handling truncated content (Common Crawl's 5 MiB limit since March 2025)
- Ensuring factual accuracy in extracted knowledge

[6] Berberich, K., et al. (2019). "Temporal Information Extraction from Web Archives"

## Recent Developments and Future Directions

### 1. Advanced Extraction Techniques

- Deep learning approaches for entity and relation extraction
- Multi-lingual information extraction
- Cross-archive entity linking
- Temporal relation extraction
- Integration with columnar storage (Parquet) for efficient indexing
- LLM-enhanced knowledge extraction and validation

[7] Zhang, Y., et al. (2022). "Deep Learning for Knowledge Graph Construction: A Survey"

### 2. Integration of LLMs and Knowledge Graphs

Recent developments have shown promising directions for combining LLMs with knowledge graphs in web archive processing:

#### a) KG-Enhanced LLMs

- Incorporating knowledge graphs during LLM pre-training
- Using knowledge graphs for inference and interpretability
- Enhancing LLM understanding of extracted knowledge

#### b) LLM-Augmented Knowledge Graphs

- Leveraging LLMs for knowledge graph construction
- Using LLMs for graph-to-text generation
- Improving question answering over web archives

#### c) Synergized LLMs + KGs

- Bidirectional reasoning between LLMs and knowledge graphs
- Mutual enhancement of both systems
- Data and knowledge-driven inference

[8] Pan, S., et al. (2024). "Unifying Large Language Models and Knowledge Graphs: A Roadmap"

### 3. Scalability Improvements

- Distributed processing frameworks
- Incremental knowledge graph updates
- Efficient storage and retrieval methods
- Parallel processing of archive files
- Columnar storage optimization for fast retrieval
- LLM-based parallel processing optimization

[9] Chen, X., et al. (2021). "Scalable Knowledge Graph Construction: A Survey"

### 4. Quality and Validation

- Entity resolution and disambiguation
- Knowledge graph validation methods
- Quality assessment metrics
- Consistency checking across archives
- LLM-based fact verification
- Cross-validation between LLMs and knowledge graphs

[10] Hogan, A., et al. (2021). "Knowledge Graph Embedding: A Survey of Approaches and Applications"

## Applications

Knowledge graphs constructed from web archives have been used in various domains:

- Historical research and analysis
- Cultural heritage preservation
- Digital humanities
- Web evolution studies
- Information retrieval and search
- Temporal trend analysis
- Link analysis and web structure studies
- LLM-enhanced web archive exploration

[11] Risse, T., et al. (2018). "Web Archive Processing: A Survey"

## Conclusion

The combination of web archives and knowledge graphs offers powerful capabilities for structured information extraction and analysis. While challenges remain in processing large-scale archives and ensuring extraction quality, ongoing developments in machine learning and distributed computing are enabling more sophisticated approaches to knowledge graph construction from web archives. The evolution of web archiving formats, particularly the specialized WET format and integration with columnar storage, continues to improve the efficiency and effectiveness of knowledge extraction from web archives. The recent integration of Large Language Models with knowledge graphs presents new opportunities for enhancing the accuracy, scalability, and interpretability of web archive information extraction.
