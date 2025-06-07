---
tags:
  - GPT
  - Benchmark
  - MMLU
  - GPQA
  - AIME
  - SWE-Bench-Verified
  - Reasoning
  - AI
  - Technologie
---
---

Step 1: Benchmark-Recherche (Prompt), o3
Step 2: Benchmark-Ergebnisse mit Kontext anreichern (Promt), GPT-4.1

---
## 1. MMLU-Pro (Massive Multitask Language Understanding)

### a. Beschreibung

**Was misst MMLU-Pro?**  
MMLU-Pro ist ein akademischer Benchmark, der breitgefächertes Wissen und Reasoning auf Hochschulniveau abprüft – von Medizin und Recht über Mathematik bis hin zu Geschichte. Die neue Pro-Version erschwert das „Prompt Engineering“ und verlangt echtes Sprachverständnis und Generalisierungsfähigkeit. Es gilt als Goldstandard für allgemeine KI-Bildung.

### b. Praxisrelevanz

**Wofür ist MMLU-Pro wirklich nützlich?**

- Wenn du ein Modell für komplexe, interdisziplinäre Recherche einsetzt, etwa für juristische oder wissenschaftliche Gutachten, medizinische Beratung (ohne Haftung), akademische Studien oder für Use Cases, bei denen breites Expertenwissen und logisches Schließen über verschiedene Fächer hinweg gefragt sind.
    
- Wähle z. B. **o3** oder **Gemini 2.5 Pro Exp** für Consulting, F&E oder rechtlich/medizinisch anspruchsvolle Zusammenhänge, weil sie stabile, nachvollziehbare Reasoning-Leistung bieten und ein sehr großes Kontextfenster für große Dokumente nutzen.
    
- **Claude 3.7 Sonnet** oder **Grok 3 Mini** sind Alternativen, wenn Tool-Integration, Multimodalität (Bilder, Text, Tabellen) oder zügige Antwortzeiten zählen.
    

### Top-10 (MMLU-Pro, Stand 05/2025)

| #   | Modell                       | Acc. % | Kontext (Tokens) | Knowledge-Cutoff | Verfügbarkeit         | Besonderheiten             |
| --- | ---------------------------- | ------ | ---------------- | ---------------- | --------------------- | -------------------------- |
| 1   | o3                           | 85.6   | 200 k            | Mai 2024         | ChatGPT / API         | starkes CoT-Reasoning      |
| 2   | Gemini 2.5 Pro Exp           | 84.1   | 1 M              | Jan 2025         | Gemini API, AI Studio | multimodal, 1 M-CTX        |
| 3   | o1                           | 83.5   | 128 k            | Okt 2023         | ChatGPT / API         | kostengünstiges Reasoning  |
| 4   | Claude 3.7 Sonnet (Thinking) | 82.7   | 200 k            | Feb 2025         | Claude.ai / API       | Hybrid-“Thinking”-Modus    |
| 5   | Grok 3 Mini Fast-High        | 81.4   | 1 M              | Okt 2024         | X Premium+ / xAI API  | reasoning & 1 M-CTX        |
| 6   | Claude 3.7 Sonnet            | 80.7   | 200 k            | Feb 2025         | Claude.ai / API       | balanced speed             |
| 7   | o4-Mini                      | 80.6   | 200 k            | Okt 2023         | ChatGPT / API         | Kosten-/Latentin-optimiert |
| 8   | GPT-4.1                      | 80.5   | 1 M              | Jun 2024         | OpenAI API            | neues Flagship, 1 M-CTX    |
| 9   | Grok 3 Mini Fast-Low         | 80.0   | 1 M              | Okt 2024         | X Premium+            | speed-maximiert            |
| 10  | Gemini 2.0 Flash Exp         | 79.2   | 1 M              | Dez 2024         | Gemini API            | Ultra-Low-Latency          |

Quelle: Vals AI MMLU-Pro Leaderboard

---

## 2. GPQA-Diamond (Graduate-Level Google-Proof Q&A)

### a. Beschreibung

**Was misst GPQA-Diamond?**  
GPQA testet „Google-resistente“ Fachfragen auf Promotionsniveau (STEM, Medizin, Wissenschaft). Im Gegensatz zu klassischen Benchmarks funktionieren reine Websuche oder Copy-Paste nicht – die Fragen zielen auf tiefes Verständnis und deduktive Logik.

### b. Praxisrelevanz

**Wofür ist GPQA-Diamond in der Praxis nützlich?**

- Optimal für alle Aufgaben, bei denen KI **echte Expertenleistung** erbringen muss: Erstellung oder Review von wissenschaftlichen Artikeln, Medizin/Gesundheitsberatung auf Expertenniveau, komplexe technische Patentanalysen, Data-Science-Consulting oder Pre-Screening von Forschungsanträgen.
    
- Für Deep-Tech-Startups oder Medizin/Forschungsunternehmen empfiehlt sich **Claude 3.7 Sonnet (Thinking)** oder **o3-mini**, weil sie den höchsten Grad an „unkopierbarer“ Problemlösung zeigen.
    

### Top-10 (GPQA-Diamond, Stand 03/2025)

|#|Modell|Acc.%|Kontext|Cutoff|Verfügbarkeit|Besonderheiten|
|---|---|---|---|---|---|---|
|1|Claude 3.7 Sonnet (Thinking)|75.3|200 k|Feb 2025|Claude API|chain-of-thought default|
|2|o3-mini|75.0|200 k|Mai 2024|ChatGPT / API|schnelle Reasoning-Variante|
|3|o1|73.0|128 k|Okt 2023|ChatGPT / API|günstiges STEM-Q&A|
|4|Claude 3.7 Sonnet|67.4|200 k|Feb 2025|Claude.ai|–|
|5|Gemini 2.0 Flash|65.2|1 M|Dez 2024|Gemini API|extrem schnell|
|6|Claude 3.5 Sonnet|59.1|200 k|Jun 2024|Claude.ai|–|
|7|Gemini 1.5 Pro|56.8|1 M|Aug 2024|Gemini API|multimodal|
|8|GPT-4o (Nov 24)|53.0|128 k|Jun 2024|ChatGPT|multimodal native|
|9|GPT-4o (Mai 24)|50.3|128 k|Jun 2024|ChatGPT|–|
|10|Gemini 1.5 Flash|49.7|1 M|Mai 2024|Gemini API|Low-cost|

Quelle: Vals AI GPQA Leaderboard

---

## 3. AIME (American Invitational Mathematics Examination)

### a. Beschreibung

**Was misst AIME?**  
AIME ist ein strenger Mathematik-Benchmark, der logische Schlussfolgerungen und kreatives Problemlösen im Stil von Mathe-Olympiaden abfragt. Er deckt anspruchsvolle Highschool- bis Undergrad-Niveau-Aufgaben ab, bei denen kein „Pattern Matching“, sondern echtes mathematisches Verstehen nötig ist.

### b. Praxisrelevanz

**Für welche Praxisprobleme ist AIME relevant?**

- Für Aufgaben in Data Science, FinTech, Physik oder Ingenieurwesen, bei denen eigenständiges mathematisches Problemlösen oder Formelableitungen gefordert sind – zum Beispiel komplexe Modellberechnungen, quantitative Investment-Analysen, Machine-Learning-Feature-Engineering, oder Wettbewerbs-Aufgaben.
    
- Wer zuverlässige mathematische Kreativleistung oder Beweisführung in der KI braucht, wählt **o3-mini** (sehr stark im Math-Reasoning) oder **o1** (Kosteneffizienz bei gleichzeitig guter Leistung).
    

### Top-10 (AIME, Stand 03/2025)

|#|Modell|Acc.%|Kontext|Cutoff|Verfügbarkeit|Besonderheiten|
|---|---|---|---|---|---|---|
|1|o3-mini|86.5|200 k|Mai 2024|ChatGPT|beste Math-Reasoning|
|2|o1|71.5|128 k|Okt 2023|ChatGPT|–|
|3|Claude 3.7 Sonnet (Thinking)|52.7|200 k|Feb 2025|Claude API|–|
|4|Gemini 2.0 Flash|29.8|1 M|Dez 2024|Gemini API|sehr schnell|
|5|Claude 3.7 Sonnet|22.5|200 k|Feb 2025|Claude.ai|–|
|6|Gemini 1.5 Pro|18.7|1 M|Aug 2024|Gemini API|–|
|7|Gemini 1.5 Flash|17.3|1 M|Mai 2024|Gemini API|Low-latency|
|8|Grok 2|15.2|128 k|Okt 2023|xAI API|–|
|9|GPT-4o|14.6|128 k|Jun 2024|ChatGPT|–|
|10|Claude 3.5 Sonnet|12.9|200 k|Jun 2024|Claude.ai|–|

Quelle: Vals AI AIME Leaderboard

---

## 4. SWE-Bench Verified (Software Engineering Benchmark)

### a. Beschreibung

**Was misst SWE-Bench?**  
SWE-Bench testet die Fähigkeit eines Modells, reale Softwarefehler (z. B. auf GitHub gemeldete Bugs) automatisiert zu erkennen und durch konkrete Code-Änderungen zu beheben. Ein Fix wird nur als „gelöst“ gewertet, wenn er im Repositorium getestet und validiert wurde – das ist einzigartig realitätsnah.

### b. Praxisrelevanz

**Wann und warum ist SWE-Bench entscheidend?**

- Für Firmen, die KI als „Developer-Agent“ einsetzen wollen – z. B. für Pull Requests, Bugfixes, Refactoring, Legacy-Migration, DevOps-Tasks oder Rapid Prototyping.
    
- Entscheidungsregel: **Nemotron-CORTEXA** für fortgeschrittene Agent-Integrationen (private Preview), **Claude 3.7 Sonnet**-basierte Systeme und **Amazon Q Dev Agent** (mit Gemini) für Unternehmen, die Enterprise-Integration und Skalierbarkeit wollen.
    

### Top-10 (SWE-Bench Verified, Stand 05/2025)

|#|System / LLM (Underlying)|% Resolved|Kontext|Cutoff|Verfügbarkeit|Besonderheiten|
|---|---|---|---|---|---|---|
|1|Nemotron-CORTEXA (NVIDIA)|68.2|128 k|Jan 2025|NVIDIA API (private preview)|Reinforcement-fine-tuned|
|2|Aime-coder v1 + Claude 3.7|66.4|200 k|Feb 2025|Agent SaaS|reasoning-agent|
|3|OpenHands (Claude 3.7)|65.8|200 k|Feb 2025|OpenHands App|code-review loop|
|4|Augment Agent (v0, Claude 3.7)|65.4|200 k|Feb 2025|closed beta|tool-use integration|
|5|Amazon Q Dev Agent (Gemini 2.0 Flash)|65.4|1 M|Dez 2024|Amazon Q|enterprise IDE plug-in|
|6|W&B Programmer o1|64.6|128 k|Okt 2023|W&B internal|offline-patch flow|
|7|PatchPilot 1.1 (GPT-4.1)|64.6|1 M|Jun 2024|patchpilot.ai|speculative-execution|
|8|AgentScope (GPT-4o)|63.4|128 k|Jun 2024|agentscope.dev|auto-PR workflow|
|9|Tools + Claude 3.7 Sonnet|63.2|200 k|Feb 2025|internal|heavy tool orchestration|
|10|Blackbox AI Agent (GPT-4o)|62.8|128 k|Jun 2024|blackboxapp.ai|commercial pay-per-fix|

Quelle: SWE-Bench Verified Leaderboard

---

## 5. Instruction Following (MultiChallenge, Scale AI)

### a. Beschreibung

**Was misst Instruction Following?**  
Benchmarks wie MultiChallenge prüfen, wie gut ein Modell komplexen Anweisungen, Workflow-Beschreibungen und verschachtelten Aufgaben folgt. Es geht nicht nur um Sprachverständnis, sondern vor allem um präzise Umsetzung mehrschrittiger Arbeitsaufträge – etwa wie gut ein Agent komplexe Tasks und Bedingungen verarbeitet.

### b. Praxisrelevanz

**Wann ist Instruction Following entscheidend?**

- In allen Bereichen, wo die KI als „Workflow-Automat“ oder Assistent Aufgaben ausführt, z. B. Customer Support, HR-Automatisierung, medizinische Dokumentation, Vertragsgenerierung, Marketing-Kampagnen oder Prozessautomatisierung.
    
- **o1** ist optimal für Unternehmen, die hochgradig zuverlässige, fehlerarme Automation in Prozessen benötigen. **Gemini 2.0 Flash** punktet, wenn Reaktionszeit (Latenz) und Skalierbarkeit im Vordergrund stehen.
    

### Top-10 (Instruction Following, Stand 03/2025)

|#|Modell|Score %|Kontext|Cutoff|Verfügbarkeit|Besonderheiten|
|---|---|---|---|---|---|---|
|1|o1 (Dec 2024)|91.96|128 k|Okt 2023|ChatGPT / API|top instruction-adherence|
|2|DeepSeek R1|87.75|128 k|Jan 2025|DeepSeek API|reasoning-focused|
|3|o1-preview|86.58|128 k|Okt 2023|API|–|
|4|Gemini 2.0 Flash Exp|86.58|1 M|Dez 2024|Gemini API|extreme speed|
|5|Claude 3.5 Sonnet|85.96|200 k|Jun 2024|Claude.ai|–|
|6|GPT-4o|85.29|128 k|Jun 2024|ChatGPT|multimodal|
|7|Gemini 1.5 Pro|84.17|1 M|Aug 2024|Gemini API|–|
|8|GPT-4 Turbo Preview|83.19|128 k|Dez 2023|OpenAI API|cost-efficient|
|9|Mistral Large 2|82.81|128 k|Nov 2024|Mistral API|French start-up|
|10|Claude 3 Opus|80.12|200 k|Feb 2024|Claude.ai|highest Claude tier|

Quelle: Scale AI Instruction-Following Leaderboard

---

## 6. Long Context Performance (LongBench v2)

### a. Beschreibung

**Was misst LongBench v2?**  
LongBench v2 bewertet, wie gut ein Modell mit sehr langen Texten/Dokumenten (teils Millionen Token) umgehen kann – z. B. „Needle in Haystack“ (Suche nach spezifischer Info), große Tabellen, Zusammenfassungen über viele Seiten hinweg oder das Erfassen und Verknüpfen von Fakten aus Langzeitkontext.

### b. Praxisrelevanz

**Wann ist Long Context relevant?**

- Für alle Aufgaben, bei denen sehr große Mengen an Kontext in einer Anfrage gebraucht werden, z. B. Due-Diligence von Verträgen (>100 Seiten), Auswertung kompletter Chatverläufe, umfangreiche Finanz- oder Tech-Reports, automatisierte Literatur-Recherche oder Zusammenfassung großer Archive.
    
- **Gemini 2.5 Pro** und **Gemini 2.5 Flash** sind führend für Aufgaben mit extrem großen Dokumenten und zeigen beste Retrieval-/QA-Performance auf bis zu 1 Million Tokens. Wer noch größere CTX (bis 4 Mio.) braucht, kann experimentell auf **MiniMax-Text-01** setzen, muss aber bei der QA-Leistung Abstriche machen.
    

### Top-10 (LongBench v2, Stand 05/2025)

|#|Modell|Overall % (w/ CoT)|Kontext|Cutoff|Verfügbarkeit|Besonderheiten|
|---|---|---|---|---|---|---|
|1|Gemini 2.5 Pro|63.3|1 M|Jan 2025|Gemini API|best long-doc QA|
|2|Gemini 2.5 Flash|62.1|1 M|Apr 2025|Gemini API|fast/cheap|
|3|DeepSeek R1|58.3|128 k|Jan 2025|DeepSeek API|open but non-OSS weights|
|4|o1-preview|57.7|128 k|Okt 2023|OpenAI API|strong retrieval|
|5|MiniMax-Text-01|52.9|4 M|Jan 2025|MiniMax API|4 M CTX (!)|
|6|Gemini 2.0 Flash-Thinking|56.0|1 M|Jan 2025|Gemini API|CoT prompt|
|7|GPT-4o|50.1|128 k|Jun 2024|ChatGPT|multimodal|
|8|Qwen3-235B-A22B|40.4|128 k|Apr 2025|Alibaba Cloud|hybrid thinking|
|9|Claude 3.5 Sonnet|41.0|200 k|Oct 2024|Claude.ai|long-dialogue strength|
|10|GLM-4 Plus|44.3|128 k|Oct 2024|Zhipu API|Chinese enterprise LLM|

Quelle: LongBench v2 Leaderboard