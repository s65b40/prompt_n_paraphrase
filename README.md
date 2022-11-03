# Prompt&Paraphrase
Repository for COLING 2022 paper "Prompt Combines Paraphrase: Teaching Pre-trained Models to Understand Rare Biomedical Words"
 
 
## Preparation for data

We conducted our experiments on two biomedical datasets **MedNLI** and **MedSTS**. Both datasets are ONLY accessible with the corresponding confidentiality agreement signed. 

### MedNLI
https://physionet.org/content/mednli/1.0.0/

### MedSTS
https://arxiv.org/abs/1808.09397

The MedSTS can be accessed by E-mail contact with the data maintainers.

## Rare biomedical words and paraphrases

As introduced in the paper, the rare biomedical words are retrieved through an API provided by an online dictionary - "[Wiktionary](https://pypi.org/project/wiktionaryparser/)". 

We consider the words with tags including 'medical', 'medicine', 'disease', 'symptom', and 'pharma-' as biomedical words. We loop through the common pre-training corpora for biomedical pre-trained models to obtain the word frequency for all possible words. Rare words are the words whose frequency in the pre-training corpora is smaller than a manually-selected threshold. Here, we provide the rare biomedical word list with a threshold of 200k and the corresponding paraphrases in the file `paraphrase.txt`.

## Questions
If you have any question about our work, feel free to open an issue or email me (`hcwang@ir.hit.edu.cn`).

## Citation
```bibtex
@inproceedings{wang-etal-2022-prompt,
    title = "Prompt Combines Paraphrase: Teaching Pre-trained Models to Understand Rare Biomedical Words",
    author = "Wang, Haochun and Liu, Chi and Xi, Nuwa and Zhao, Sendong and Ju, Meizhi and Zhang, Shiwei and Zhang, Ziheng and Zheng, Yefeng and Qin, Bing and Liu, Ting",
    booktitle = "Proceedings of the 29th International Conference on Computational Linguistics",
    month = oct,
    year = "2022",
    address = "Gyeongju, Republic of Korea",
    publisher = "International Committee on Computational Linguistics",
    url = "https://aclanthology.org/2022.coling-1.122",
    pages = "1422--1431",
    
}
```


