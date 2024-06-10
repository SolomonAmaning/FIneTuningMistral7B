# FIne Tuning Mistral7B


The purpose of this project was to improve the output of discharge summaries using Mistral 7B. 
Mistral was originally trained on PubMed data.
In a clinical setting, discharge summaries should follow a specific template, the SOAP template (Subjective, Objective, Assessment, Plan).

To ensure that the discharge summary output follows this structure, we needed to fine-tune the model with data that exhibits these characteristics. 
For this fine-tuning process, we used the "mts-dataset-clinical-dialogue-and-summary" available on HuggingFace.
As the name suggests, this dataset summarizes important patient-doctor dialogues under headings including symptoms, medical history, family history, assessment, and investigations.

After tuning, the language model was prompted to generate completions based on the different  prompts to assess the precision of the completion compared to the referenced input text.


