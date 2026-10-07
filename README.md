# Awesome-Optical-Character-Recognition-Ocr-Document-AI

## Top Optical Character Recognition (OCR) & Document AI Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**  

*Focused on Document Parsing, Structured Extraction & Self-Hosted OCR Engines*  

**Last updated: October 2026**



This repository tracks notable **commercial OCR and Document AI platforms** and **open-source projects** that extract text, tables, and structured data from documents — invoices, receipts, contracts, forms, and scanned PDFs — using OCR, layout analysis, and vision-language models.



**Examples** include Amazon Textract, Google Cloud Document AI, Azure AI Document Intelligence, ABBYY Vantage, Rossum, Klippa DocHorizon, Hyperscience, Nanonets, Base64.ai, and Veryfi (the category leaders).



**Open-source emphasis**: Document AI is one of the strongest open-source domains in 2026. **Docling** (IBM Research) leads as the self-hostable alternative to cloud Document AI. **PaddleOCR-VL** and **Qianfan-OCR** achieve state-of-the-art parsing accuracy. **Tesseract** remains the veteran OCR engine, **EasyOCR** simplifies multilingual OCR, and **Surya** delivers layout and table recognition. **lift** and **NuExtract3** enable schema-constrained extraction. **olmOCR** handles industrial-scale PDF digitization. This section is heavily expanded.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saas-hosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **[Amazon Textract](https://aws.amazon.com/textract/)**  

  **AWS's document text and data extraction service** — forms, tables, and structured data using ML . **Best for AWS-native document processing** .



- **[Google Cloud Document AI](https://cloud.google.com/document-ai)**  

  **Google's document understanding platform** — pre-trained models for invoices, receipts, forms, and custom extraction . **Best for GCP-native document AI** .



- **[Azure AI Document Intelligence](https://azure.microsoft.com/en-us/products/ai-services/ai-document-intelligence)**  

  **Microsoft's document processing service** — pre-built and custom extraction models . **Best for Azure-native document AI** .



- **[ABBYY Vantage](https://www.abbyy.com/)**  

  **Intelligent document processing platform** — OCR, classification, and extraction with human-in-the-loop . **Best for enterprise document automation** .



- **[Rossum](https://rossum.ai/)**  

  **AI-powered document automation** — invoice and purchase order processing with transactional focus . **Best for invoice automation** .



- **[Klippa DocHorizon](https://www.klippa.com/)**  

  **Document automation platform** — OCR and data extraction for receipts, invoices, and identity documents . **Best for financial document processing** .



- **[Hyperscience](https://www.hyperscience.com/)**  

  **Enterprise intelligent document processing** — human-in-the-loop automation for complex documents . **Best for complex document workflows** .



- **[Nanonets](https://nanonets.com/)**  

  **No-code AI document processing** — invoices, receipts, and forms with pre-built and custom models . **Best for no-code document AI** .



- **[Base64.ai](https://base64.ai/)**  

  **Document AI platform** — 500+ document types with pre-trained extraction . **Best for multi-document processing** .



- **[Veryfi OCR API](https://www.veryfi.com/)**  

  **Real-time document extraction API** — receipts, invoices, and financial documents with mobile SDKs . **Best for financial document processing** .



## Open-Source GitHub Projects



### Document AI Frameworks



- **[Docling](https://github.com/docling-project/docling)**  

  **The leading open-source document processing framework from IBM Research**, MIT licensed . **Thoughtworks Technology Radar calls it "an open-source, self-hostable alternative to proprietary cloud-managed services such as Azure Document Intelligence, Amazon Textract and Google Document AI"** . **Converts complex PDFs and scanned documents into structured JSON and Markdown** using computer vision-based layout and semantic understanding . **Strong for RAG pipelines with reading order preservation, table structure recognition, and visual grounding** . Integrates with LangChain and LangGraph . **The de facto open-source Document AI framework** . **Best for self-hosted document processing** .



### OCR Engines



- **[Tesseract OCR](https://github.com/tesseract-ocr/tesseract)**  

  **The foundational open-source OCR engine**, Apache-2.0 licensed with **60,000+ GitHub stars** . **Supports 100+ languages** . **LSTM-based recognition** . **The most widely deployed OCR engine** . **Best for general OCR** .



- **[EasyOCR](https://github.com/JaidedAI/EasyOCR)**  

  **Ready-to-use OCR with 80+ languages**, Apache-2.0 licensed with **25,000+ GitHub stars** . **Simple Python API** . **Best for multilingual OCR** .



- **[PaddleOCR-VL-1.6](https://huggingface.co/PaddlePaddle/PaddleOCR-VL-1.6)**  

  **Baidu's compact document parsing model achieving 96.33% on OmniDocBench v1.6** — state-of-the-art among open-source solutions . **1B parameter model with region-aware optimization and seal/stamp recognition** . Apache-2.0 licensed . **Best for state-of-the-art document parsing** .



- **[Qianfan-OCR](https://huggingface.co/rootlocalghost/Qianfan-OCR)**  

  **Baidu Qianfan Team's 4B-parameter end-to-end document intelligence model** — **#1 end-to-end model on OmniDocBench v1.5** (93.12 overall), surpassing DeepSeek-OCR-v2 (91.09) and Gemini-3 Pro (90.33) . **192 languages supported** . **Layout-as-Thought phase for structured layout recovery** . **Best for high-accuracy multilingual parsing** .



- **[Surya](https://github.com/VikParuchuri/surya)**  

  **Document OCR, layout, and tables via 0.7B parameter model** . **Best for layout-aware OCR** .



- **[RapidOCR](https://github.com/RapidAI/RapidOCR)**  

  **Cross-platform OCR based on PaddleOCR models** — runs on CPU with ONNX Runtime . **Best for lightweight OCR** .



- **[TrOCR](https://github.com/microsoft/unilm/tree/master/trocr)**  

  **Transformer-based OCR from Microsoft** — combines vision and language models . **Best for handwritten text** .



### Structured Extraction



- **[lift](https://huggingface.co/datalab-to/lift)**  

  **Structured extraction model from Datalab** — pulls structured JSON from PDFs and images using **schema-constrained decoding** to guarantee valid, well-typed output . **90.2% field accuracy with 9.5s median latency** . **Handles multi-page documents and values spanning pages** . Apache 2.0 code with modified OpenRAIL-M weights . **Best for schema-constrained extraction** .



- **[NuExtract3](https://huggingface.co/numind/NuExtract3)**  

  **NuMind's structured extraction model** — supports in-context examples and template generation from natural language . **81.5% field accuracy, 8.3s median latency** (fastest local model tested) . **Best for flexible extraction** .



- **[DocTR](https://github.com/mindee/doctr)**  

  **OCR library with structured JSON output** — blocks, lines, words, and bounding boxes . **PyTorch and TensorFlow support** . **Best for OCR-first pipelines** .



### PDF Conversion & Parsing



- **[Marker](https://github.com/VikParuchuri/marker)**  

  **Convert PDF to Markdown and JSON**, GPL-3.0 licensed with **20,000+ GitHub stars** . **Fast and accurate PDF conversion** . **Best for PDF ingestion** .



- **[olmOCR](https://github.com/allenai/olmocr)**  

  **Allen AI's industrial-scale PDF digitization tool** achieving **82.4% on olmOCR-bench** . **Converts one million PDF pages for ~$190** — roughly 1/32nd the cost of GPT-4o . **7B model requires NVIDIA GPU with 16GB+ VRAM** . **Best for high-volume digitization** .



- **[PyMuPDF](https://github.com/pymupdf/PyMuPDF)**  

  **PDF parsing and manipulation**, AGPL-3.0 licensed . **High-performance PDF processing** . **Best for PDF extraction** .



- **[Tika](https://github.com/apache/tika)**  

  **Apache content analysis toolkit** — extracts text and metadata from 1,000+ file types . **Best for universal document parsing** .



### Compact & Edge OCR



- **[TinyDoc-VLM](https://pypi.org/project/tinydoc-vlm/)**  

  **256M-parameter document-specialist VLM** — runs on **CPU, Raspberry Pi 5, or MacBook Air with <1GB VRAM** . **Handles invoices, receipts, forms, tables, and charts** . Apache 2.0 licensed with ONNX export and LoRA fine-tuning . **Best for edge and low-resource OCR** .



- **[docTR](https://github.com/mindee/doctr)** — Already listed. **Lightweight OCR** .



### Additional Strong Open-Source Options



- **MonkeyOCRv2** — 0.8B parsing model with smaller and larger variants .

- **MinerU2.5** — OpenDataLab's 1.2B structured JSON/Markdown extraction pipeline .

- **Kreuzberg** — Document extraction engine supporting 101 formats .

- **AlienTables** — Local, privacy-first PDF-to-Excel extraction .

- **VerifyDoc** — Trust layer for AI document extraction .

- **Receipt Wrangler** — Self-hosted receipt tracking with OCR .

- **OpenOCR** — Open-source OCR toolkit .

- **OCRmyPDF** — Add OCR layer to PDFs .



**Frameworks for building custom OCR and Document AI solutions**: Combine **Docling** for layout-aware parsing and RAG-ready output . Use **PaddleOCR-VL-1.6** or **Qianfan-OCR** for state-of-the-art parsing accuracy . Deploy **Tesseract** or **EasyOCR** for general and multilingual OCR . Choose **lift** or **NuExtract3** for schema-constrained structured extraction . Integrate **Marker** or **olmOCR** for PDF conversion and high-volume digitization . Use **TinyDoc-VLM** for edge and CPU-only deployments . Note that true enterprise Document AI with managed scaling, pre-built industry models, and compliance certifications remains primarily commercial territory; open-source stacks provide strong parsing, extraction, and validation foundations that require integration for complete document automation.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- OCR and Document AI platforms process potentially sensitive documents including financial records, contracts, and personal data. Self-hosted solutions require proper security hardening, access controls, and compliance with data privacy regulations (GDPR, CCPA, HIPAA).

- **Model accuracy varies by document type, language, and quality** — benchmark results should not be interpreted as guarantees of production performance on your specific documents . Validate on your own data before deployment.

- **License considerations**: Docling uses MIT, Tesseract uses Apache-2.0, PaddleOCR-VL uses Apache-2.0, Marker uses GPL-3.0, and lift uses Apache 2.0 with modified OpenRAIL-M weights. Verify licensing against your use case before committing .

- **Hardware requirements vary significantly** — TinyDoc-VLM runs on Raspberry Pi with <1GB VRAM; olmOCR needs NVIDIA GPU with 16GB+ VRAM . Plan infrastructure accordingly .

- The open-source ecosystem provides strong parsing, extraction, and validation foundations, but **managed scaling, industry-specific pre-trained models, and compliance certifications** remain primarily commercial offerings.



---



**Made for document processing engineers, automation architects, and organizations seeking Document AI sovereignty.**  

Let's make optical character recognition and Document AI more open, transparent, and accurate.
