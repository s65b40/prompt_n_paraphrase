# Prompt&Paraphrase
Repository for COLING 2022 paper "Prompt Combines Paraphrase: Teaching Pre-trained Models to Understand Rare Biomedical Words"
 
 
## Preparation for data

We conducted our experiments on two biomedical datasets **MedNLI** and **MedSTS**. Both datasets are ONLY accessible with the corresponding confidentiality agreement signed. 

### MedNLI
https://physionet.org/content/mednli/1.0.0/

###MedSTS
https://arxiv.org/abs/1808.09397

The MedSTS can be accessed by E-mail contact with the data maintainers.

## Rare biomedical words and paraphrases

As introduced in the paper, the rare biomedical words are retrieved through an API provided by an online dictionary - "[Wiktionary](https://pypi.org/project/wiktionaryparser/)". 

We consider the words with tags including 'medical', 'medicine', 'disease', 'symptom', and 'pharma-' as biomedical words. We loop through the common pre-training corpora for biomedical pre-trained models to obtain the word frequency for all possible words. Rare words are the words whose frequency in the pre-training corpora is smaller than a manually-selected threshold. Here, we provide the rare biomedical word list with a threshold of 200k and the corresponding paraphrases in the file `paraphrase.txt`.



