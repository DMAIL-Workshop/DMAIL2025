---
layout: page
title: Legal Bias Flagging Challenge
permalink: /lbc/
order: 2
---

The Legal Bias Flagging Challenge is a new feature of DMAIL 2025, designed to advance the field of responsible and explainable AI in law. This competition invites participants to tackle the important task of flagging bias in legal texts, an issue that lies at the heart of fairness and accountability in automated legal systems.
    
# **Challenge Overview**

<div style="text-align: justify">Participants will develop models that automatically detect and explain potential bias in passages from legal case texts. Each task instance will include: </div> 


-   a highlighted passage potentially containing bias, 
-   the full case text for broader contextual understanding, 
-   and a language column. 


The model must output a **binary decision (Y/N)** indicating whether the passage contains bias, along with an automatically generated explanation justifying the prediction. This dual-output task emphasizes both performance and interpretability.

For this challenge, **bias** is defined as follows (based on an excerpt from this dictionary https://dictionary.law.com/Default.aspx?selected=61):
*the predisposition of a judge, arbitrator, prospective juror, or anyone making a judicial decision, against or in favor of one of the parties or a class of persons. This can be shown by remarks, decisions contrary to fact, reason or law, or other unfair conduct.* 


# **Dataset and Setup**

The dataset consists of legal cases from a range of jurisdictions, including the United States, Germany, Japan, Vietnam, and Korea. To encourage innovative and adaptable approaches, the challenge will not include any labeled training data. Participants are expected to develop their models using their own methodologies, publicly available resources, and general knowledge.

# **Evaluation and Awards**

All submissions will be evaluated against a hidden ground truth curated by the DMAIL organizing team. The primary evaluation metric will be the F2-score, which places greater emphasis on recall for detecting biased passages.

Winners will be announced in two categories:

-   The **Overall Winner**, awarded to the top-performing model on the challenge dataset.
-   The **Low-Resource Setting Winner**, awarded to the best-performing system operating under constrained computing resources.



To qualify for the low-resource category, participants must use publicly available pre-trained models (e.g., from HuggingFace or Ollama), and meet at least one of the following criteria: 


-   the model must contain no more than 100 million parameters, or 
-   it must run using no more than 16 GB of VRAM. 


Submissions in this category must also include a short description of the experimental setup, including model architecture and size, hardware and VRAM usage, the used prompt(s) and overall methodology.


# **Why Participate?**

This challenge offers participants the opportunity to work with diverse, multilingual legal datasets while addressing a critical ethical issue in legal AI. It provides a platform to benchmark models in a realistic and challenging scenario and gain visibility at an international workshop co-located with IEEE ICDM.

Participants are also encouraged to submit a short paper describing their method, results, and insights. Papers should be no more than 4 pages in length and must follow the standard two-column U.S. letter IEEE conference format. See the IEEE Proceedings Author Guidelines for formatting instructions. Authors of accepted papers must present their work at the DMAIL 2025 workshop to have their paper included in the official workshop proceedings.


# **Participation Requirements**

To participate in the Legal Bias Flagging Challenge, each team must complete a formal registration process prior to gaining access to the dataset.

Participation requires:


-   Signing a license agreement, which outlines the permitted use of the challenge data ([DMAIL_Challenge_Memorandum_Form_2025.pdf](https://drive.google.com/file/d/1m4Hc3J2UtDPrXGHK77lYa6fNcgxv4WMd/view?usp=sharing))
-   Submitting a registration form, which must list all team members involved in the project ([DMAIL_Challenge_Registration_Form_2025.pdf](https://drive.google.com/file/d/1Bj8MpZonMrulfumhNJ7413xOkxvj_WxE/view?usp=sharing))


Only teams that have completed the registration form and signed the license agreement will be granted access to the dataset and permitted to submit challenge results.


# **Submission Instructions**

Each participant must submit two plain text (.txt) files:

-   **Predictions File**
    A plain text file with one line per prediction in the following format: `instance_id, label, explanation`
    -   `instance_id`: Provided with each task example
    -   `label`: “Y” (biased) or “N” (not biased)
    -   `explanation`: A brief, automatically generated justification
-   **System Description File**
    A separate `.txt` file describing:
    -   Prompt (if used)
    -   Model name, size, and availability
    -   Hardware setup and VRAM usage
    -   A concise summary of the overall methodology


All files must be submitted via email by the deadline.


# **Important Dates**

-   Challenge Registration Opens: August 10, 2025
-   Dataset Release: August 12, 2025
-   Submission Deadline: August 30, 2025
-   Results Announcement: September 1, 2025
-   Challenge Paper Submission Deadline: September 5, 2025
-   Notification to Authors: September 18, 2025
-   Camera-Ready Deadline: September 25, 2025
-   Workshop Date: November 12, 2025


