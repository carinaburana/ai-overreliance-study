# AI Overreliance Study: Data & Analysis

This repository contains anonymized interaction logs and survey data from a user study ($N = 17$) investigating human trust, verification behavior, and overreliance in Conversational AI.

## Repository Overview

The study evaluates user behavior across **4 experimental conditions/groups** (between-subjects / within-subjects setup across two task conditions). Data collection combines real-time UI/database interaction logs with post-interaction survey measurements.

Participant identifiers are pseudonymized consistently across both primary CSV files (`interaction_data_clean.csv` and `quiz_results_clean.csv`).

---

## Files & Data Structure

### 1. `interaction_data_clean.csv`
Contains granular interaction telemetry recorded during user sessions:
* **Overreliance & Error Acceptance:** Operationalized as the **error adoption rate** (*Fehlerübernahmerate*), measuring whether participants accepted incorrect AI-generated responses.
* **Verification Behavior (*Verifikationsverhalten*):** Automatically tracked via participant actions:
  * Click events on source links (*Klicks auf Quellenlinks*)
  * Source link hovering for $\ge 200\text{ ms}$ (based on Koivisto & Grassini, 2016)
  * Text selection / copying of answer fragments (*Kopieren von Antwortteilen*)

### 2. `quiz_results_clean.csv`
Contains survey responses and psychometric scale evaluations:
* **Trust in Automation (S-TiAS):** Measured using the Short Trust in Automated Systems scale (McGrath et al., 2025; 3 items on a 7-point Likert scale) across 3 measurement intervals:
  1. Baseline (pre-task)
  2. Post-Condition 1
  3. Post-Condition 2
* **Need for Cognition (NFC-K):** Measured using the German Short Scale for Need for Cognition (*Deutschsprachige Kurzskala zur Messung des Konstrukts Need for Cognition*, Beißert et al., 2015; 4 items on a 7-point Likert scale).
* **Demographics & Accuracy Metrics:** Participant background information and task performance/decision accuracy scores.

---

## Experimental Setup & Methodology

* **Sample Size:** $N = 17$ participants assigned across 4 experimental groups.
* **Study Design:** Wizard-of-Oz experimental framework exploring how interaction design affects user reliance on AI assistants.
* **Data Anonymization:** All personal identifiers have been pseudonymized and stripped of PII.

---

## References & Validated Measures

* **Koivisto, M., & Grassini, S. (2016).**  Neural processing around 200 ms after stimulus-onset correlates with subjective visual awareness. Neuropsychologia, 84:235–243. [https://doi.org/10.1016/j.neuropsychologia.2016.02.024](https://doi.org/10.1016/j.neuropsychologia.2016.02.024)
* **McGrath et al. (2025).**  Measuring trust in artificial intelligence: Validation of an established scale and its short form. Frontiers in Artificial Intelligence,
8:1582880. [https://doi.org/10.3389/frai.2025.1582880](https://doi.org/10.3389/frai.2025.1582880) 
* **Beißert, H., Köhler, M., Rempel, M., & Beierlein, C. (2015).** *Deutschsprachige Kurzskala zur Messung des Konstrukts Need for Cognition (NFC-K)*. ZIS – Zusammenstellung sozialwissenschaftlicher Items und Skalen. [https://doi.org/10.6102/zis230](https://doi.org/10.6102/zis230)

---

## Citation

If you use this dataset or operationalization framework in your research, please cite:

```bibtex
@thesis{wiedemann2026overreliance,
  author       = {Carina Wiedemann},
  title        = {Overreliance in Human-AI Interaction: Designing for Appropriate Reliance on Conversational Agents},
  school       = {Technische Hochschule Ingolstadt},
  year         = {2026},
  type         = {Bachelor's Thesis}
}
