[![Encyclopedia of Arabic Rhetoric](static/logo.png "Encyclopedia of Arabic Rhetoric.")](https://al-balagha.com)
# [Arabic Rhetorical Device Identifier (v0.1.0)](https://github.com/Al-Balagha/Arabic-Rhetoric-Identifier/tree/v0.1.0)
### A project of the [Encyclopedia of Arabic Rhetoric](https://al-balagha.com)

A custom GPT and AI system prompt package to assist in identifying Arabic rhetorical devices, in classical and contemporary Arabic texts, published by the [Encyclopedia of Arabic Rhetoric](https://al-balagha.com).


[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.18236000.svg)](https://doi.org/10.5281/zenodo.18236000)

&nbsp;
## ℹ️ About
The Arabic Rhetorical Device Identifier (ARDI) is a digital humanities research artefact designed to support the systematic identification of Arabic rhetorical devices in classical and contemporary Arabic texts using the [Arabic Rhetorical Device Taxonomy](https://al-balagha.com/wiki/Arabic_Rhetorical_Device_Taxonomy) developed by the [Encyclopedia of Arabic Rhetoric](https://al-balagha.com/).

The ARDI consists of a custom Generative Pre-trained Transformer (GPT) interface and artificial intelligence (AI) system prompts which create a human-in-the-loop AI-assisted analytical framework, enabling transparent and reproducible rhetorical analysis. The ARDI allows for different levels of sensitivity in detecting rhetorical devices, and can be used for Arabic texts of any genre and dialect. It is designed to assist researchers, students, and annotators by highlighting candidate rhetorical devices in Arabic texts for subsequent human evaluation. The ARDI incorporates the [Arabic Rhetorical Device Taxonomy v0.1.1](https://github.com/Al-Balagha/Arabic-Rhetoric/tree/v0.1.1) and can be used as an operational interface to the Taxonomy.

Additionally, the ARDI includes a mode where users can interrogate the [Arabic Rhetorical Device Taxonomy](https://al-balagha.com/wiki/Arabic_Rhetorical_Device_Taxonomy) through an AI interface, a mode where the ARDI offers a conversation about the [Arabic Rhetorical Device Taxonomy](https://al-balagha.com/wiki/Arabic_Rhetorical_Device_Taxonomy), and a mode where the ARDI offers users a rhetorical device identification game which can be set at different levels of difficulty.

The ARDI is freely released under the CC-BY 4.0 license to promote the development of contemporary Arabic rhetorical studies, and is currently being used by the [**BALAGHA Score**](https://balaghascore.com) and [other projects](https://project.balaghascore.com).


&nbsp;
## 🎯 Purpose
The ARDI is designed to:

* Assist in identifying rhetorical devices in Arabic texts.
* Reduce omission bias during manual annotation.
* Provide structured explanations aligned with classical Arabic rhetoric.
* Support reproducible, transparent rhetorical analysis workflows.
* Support education about Arabic rhetorical devices.
* Support training in Arabic rhetorical device identification through a gamified challenge mode.


&nbsp;
## 📦 Repository Contents
The ARDI package is self-contained and has been tested with the following AI systems: OpenAI ChatGPT, Anthropic Claude, and Google Gemini. No executable code is included; the ARDI is platform-agnostic. While outputs may vary across AI models, the ARDI's analytical behaviour is governed by explicit system instructions and taxonomy constraints rather than model-specific heuristics.

The package provides three formally equivalent distributions of the ARDI which differ only in delivery format and usability constraints, not in theoretical scope, taxonomy, or methodological assumptions.

Users may select the distribution most appropriate to their technical context:

### 1️⃣ `CUSTOM_GPT/` — Platform-integrated configuration
A complete ARDI implementation packaged for use as a custom GPT, including system instructions, operational modes, and the rhetorical taxonomy.

* Optimised for interactive analysis, teaching, and live demonstrations.
* Requires a platform that supports custom GPT deployment.
* Behaviour is methodologically identical to the standalone system prompt.

### 2️⃣ `CUSTOM_PROMPT_FULL/` — Standalone system prompt
A single, self-contained system prompt reproducing the full ARDI behaviour across all modes.

* Platform-agnostic and suitable for long-term archiving.
* Recommended for reproducible research, peer review, and citation.
* Independent of proprietary interfaces or UI constraints.

### 3️⃣ `CUSTOM_PROMPTS_LITE/` — Mode-specific prompts for constrained environments
Four scope-limited variants of the ARDI system prompt, each corresponding to a single operational mode.

* Designed for limited context windows or reduced memory environments.
* Preserves conceptual consistency with the full system.
* Intended for rapid analysis, experimentation, or accessibility‑restricted accounts.

All distributions instantiate the same rhetorical taxonomy, analytical logic, and human-in-the-loop design philosophy.


&nbsp;
## 📚 Folder structure
```
/
├── README.md
├── LICENSE.txt
├── CITATION.cff
├── CHANGELOG.md
│
├── static/
│   └── logo.png
│
├── CUSTOM_GPT/
│   ├── 00_SYSTEM_INSTRUCTIONS.txt
│   ├── 01_MODES.txt
│   ├── 02_TAXONOMY.md
│   └── README.md
│
├── CUSTOM_PROMPT_FULL/
│   ├── ARABIC_RHETORICAL_DEVICE_IDENTIFIER_CUSTOM_PROMPT.txt
│   └── README.md
│
└── CUSTOM_PROMPTS_LITE/
    ├── 00_ARABIC_RHETORICAL_DEVICE_IDENTIFIER_CUSTOM_PROMPT_ANALYSIS.txt
    ├── 01_ARABIC_RHETORICAL_DEVICE_IDENTIFIER_CUSTOM_PROMPT_EXPLAIN.txt
    ├── 02_ARABIC_RHETORICAL_DEVICE_IDENTIFIER_CUSTOM_PROMPT_CONVERSATION.txt
    ├── 03_ARABIC_RHETORICAL_DEVICE_IDENTIFIER_CUSTOM_PROMPT_CHALLENGE.txt
    └── README.md

```

&nbsp;
## 📋 Prerequisites
* Access to an AI platform such as ChatGPT, Claude, or Gemini.
* Basic understanding of how to use the AI platform.


&nbsp;
## 🚀 Quick Start
1. Choose your distribution (Custom GPT or Standalone Prompt).
2. Upload to your preferred AI platform.
3. Start with "Run this prompt" or use conversation starters.


&nbsp;
## ▶️ How to Use
The ARDI can be used in two environments which behave identically by design:

### 1️⃣ As a Custom GPT

* Upload the contents of [/CUSTOM_GPT/00_SYSTEM_INSTRUCTIONS.txt](/CUSTOM_GPT/00_SYSTEM_INSTRUCTIONS.txt) to a Custom GPT configuration, and add the files [/CUSTOM_GPT/01_MODES.txt](/CUSTOM_GPT/01_MODES.txt) and [/CUSTOM_GPT/02_TAXONOMY.md](/CUSTOM_GPT/02_TAXONOMY.md) as knowledge files.
* Users interact via pre-defined conversation starters or free input.
* Best suited for demonstrations, teaching, and guided analysis.

### 2️⃣ As a Stand‑alone Prompt

* Upload a custom prompt file into a standard AI chat interface and start the conversation with an AI chat command such as "Run this prompt":
  * The file [/CUSTOM_PROMPT_FULL/ARABIC_RHETORICAL_DEVICE_IDENTIFIER_CUSTOM_PROMPT.txt](/CUSTOM_PROMPT_FULL/ARABIC_RHETORICAL_DEVICE_IDENTIFIER_CUSTOM_PROMPT.txt) contains all 4 modes and is the most comprehensive and recommended prompt file.
  * The following files each encode one mode of the ARDI, which may be more suitable for limited context windows or reduced memory environments:
    * [/CUSTOM_PROMPTS_LITE/00_ARABIC_RHETORICAL_DEVICE_IDENTIFIER_CUSTOM_PROMPT_ANALYSIS.txt](/CUSTOM_PROMPTS_LITE/00_ARABIC_RHETORICAL_DEVICE_IDENTIFIER_CUSTOM_PROMPT_ANALYSIS.txt) - Analysis mode.
    * [/CUSTOM_PROMPTS_LITE/01_ARABIC_RHETORICAL_DEVICE_IDENTIFIER_CUSTOM_PROMPT_EXPLAIN.txt](/CUSTOM_PROMPTS_LITE/01_ARABIC_RHETORICAL_DEVICE_IDENTIFIER_CUSTOM_PROMPT_EXPLAIN.txt) - Explanation mode.
    * [/CUSTOM_PROMPTS_LITE/02_ARABIC_RHETORICAL_DEVICE_IDENTIFIER_CUSTOM_PROMPT_CONVERSATION.txt](/CUSTOM_PROMPTS_LITE/02_ARABIC_RHETORICAL_DEVICE_IDENTIFIER_CUSTOM_PROMPT_CONVERSATION.txt) - Conversation mode.
    * [/CUSTOM_PROMPTS_LITE/03_ARABIC_RHETORICAL_DEVICE_IDENTIFIER_CUSTOM_PROMPT_CHALLENGE.txt](/CUSTOM_PROMPTS_LITE/03_ARABIC_RHETORICAL_DEVICE_IDENTIFIER_CUSTOM_PROMPT_CHALLENGE.txt) - "Arabic rhetorical device identification challenge" game.
	
* Suitable for archival, reproducible, and citable workflows.


&nbsp;
## ⚠️ Limitations
* AI-assisted identification requires human verification.
* Output quality depends on underlying AI model capabilities.
* The ARDI is not a replacement for expert human annotation.
* Classical vs. contemporary rhetorical interpretations may vary


&nbsp;
## 🔄 Versioning
The ARDI uses **Semantic Versioning (SemVer)**.

* **v0.1.0 (13 January 2025)**
  First public release. Includes:

  * Core system instructions.
  * Mode-based behaviour control.
  * Integration with the [Arabic Rhetorical Device Taxonomy v0.1.1](https://github.com/Al-Balagha/Arabic-Rhetoric/tree/v0.1.1).


&nbsp;
## 🤝 How to contribute
This is a research artefact with versioned releases. Please contact the author for any suggestions or issues.


&nbsp;
### 📖 How to Cite
**APA:**
Marathe, M. (2025). *Arabic Rhetorical Device Identifier (ARDI) (v0.1.0)*. Encyclopedia of Arabic Rhetoric. [https://doi.org/10.5281/zenodo.18236000](https://doi.org/10.5281/zenodo.18236000)

**Chicago:**
Marathe, Mandar. *Arabic Rhetorical Device Identifier (ARDI), v0.1.0*. Encyclopedia of Arabic Rhetoric, 2025. [https://doi.org/10.5281/zenodo.18236000](https://doi.org/10.5281/zenodo.18236000)

**BibTeX:**

```bibtex
@software{ardi2025,
  author  = {Mandar Marathe},
  title   = {Arabic Rhetorical Device Identifier (ARDI)},
  year    = {2025},
  version = {0.1.0},
  url     = {https://doi.org/10.5281/zenodo.18236000}
}
```


&nbsp;<br>
---
## 📬 About the Author
**[Dr Mandar Marathe](https://marathe.org)** | [SOAS Profile](https://www.soas.ac.uk/about/mandar-marathe)  
PhD Researcher in Arabic Rhetoric | SOAS University of London  
[![Project Home](https://img.shields.io/badge/BALAGHA%20Score%20Project-Home-green)](https://project.balaghascore.com)  

### Related Projects
- 📚 [Encyclopedia of Arabic Rhetoric](https://al-balagha.com) - Reference source for Arabic rhetorical devices  
- 💯 [BALAGHA Score](https://balaghascore.com) - Arabic rhetorical density analysis  
- 📖 [Balagha Corpus](https://balagha-corpus.com) - Annotated texts for Arabic rhetorical analysis  
- 📡 [BalaghaBase.org](https://balaghabase.org) - Semantic knowledge graph for Arabic rhetoric  
- 🔬 [Rhetorical Density](https://rhetorical-density.com) - Methodology and discussion of rhetorical density as a quantitative metric  

### Connect
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Profile-blue)](https://www.linkedin.com/in/mandar-marathe-uk/) [![ORCID](https://img.shields.io/badge/ORCID-Profile-green.svg)](https://orcid.org/0000-0002-6927-6836) [![Google Scholar](https://img.shields.io/badge/Google%20Scholar-Profile-blue)](https://scholar.google.com/citations?user=w-bT-iYAAAAJ)  
---
_Last updated: 13 January 2025._
