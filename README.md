# FORK: Food ORiented cultural commonsense Knowledge

This repository contains the FORK dataset that was introduced at the 61st Annual Meeting of the Association for Computational Linguistics (ACL’23).

Full details about the paper can be found in our Findings paper: [FORK: A Bite-Sized Test Set for Probing Culinary Cultural Biases in Commonsense Reasoning Models](https://shramay-palta.github.io/assets/pdf/FORK_ACL2023/paper.pdf)

## Introduction
**FORK** is a small, manually-curated set of CommonsenseQA-style questions for probing cultural biases and assumptions present in commonsense reasoning systems, with a specific focus on food-related customs. 

All questions were written in **English**.

## Dataset
The dataset is released in both `JSONL` and `CSV` formats. FORK contains `184` CommmonsenseQA-style questions. 

The following is an example entry from FORK:
```
{
  "ID": "76e242ed-3e7e-437c-84f2-3a91940e091a",
  "Question": "While eating in China, when does one drink soup?",
  "Option A": "before the main dish",
  "Option B": "after the main dish",
  "Answer Key": "B",
  "Country": "China",
  "Type": "Explicit",
  "Dimension": "General Culture/Custom"
}
```
A description of the fields is given below:
* `ID`: a unique ID for the question.
* `Question`: the question (in English).
* `Option A`: the first option.
* `Option B`: the second option.
* `Answer Key`: the correct answer.
* `Country`: the country to which the question pertains.
* `Type`: the type of question (explicit, implicit or underspecified.)
* `Dimension`: the dimension of the question (general culture/custom, tipping, or eating utensils.)
## License
This project is licensed under the CC-BY-4.0 License.
## Citation
If you use this dataset, please cite the following paper:
```
@inproceedings{palta-rudinger-2023-fork,
    title = "{FORK}: A Bite-Sized Test Set for Probing Culinary Cultural Biases in Commonsense Reasoning Models",
    author = "Palta, Shramay  and
      Rudinger, Rachel",
    booktitle = "Findings of the Association for Computational Linguistics: ACL 2023",
    month = jul,
    year = "2023",
    address = "Toronto, Canada",
    publisher = "Association for Computational Linguistics",
    url = "https://aclanthology.org/2023.findings-acl.631",
    pages = "9952--9962",
    abstract = "It is common sense that one should prefer to eat a salad with a fork rather than with a chainsaw. However, for eating a bowl of rice, the choice between a fork and a pair of chopsticks is culturally relative. We introduce FORK, a small, manually-curated set of CommonsenseQA-style questions for probing cultural biases and assumptions present in commonsense reasoning systems, with a specific focus on food-related customs. We test several CommonsenseQA systems on FORK, and while we see high performance on questions about the US culture, the poor performance of these systems on questions about non-US cultures highlights systematic cultural assumptions aligned with US over non-US cultures.",
}
```