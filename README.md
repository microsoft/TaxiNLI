# TaxiNLI

![Alt text](taxonomy.png?raw=true "A Taxonomy of Reasoning Capabilities")

We release TaxiNLI dataset associated with [TaxiNLI: Taking a ride up the NLU Hill](https://www.aclweb.org/anthology/2020.conll-1.4.pdf) ([CoNLL 2020 Talk](https://slideslive.com/38939466/taxinli-taking-a-ride-up-the-nlu-hill)). Essentially each row in this data corresponds to an NLI example in the MultiNLI dataset (can be identified using pairID and genre). We add 18 features, namely:
- Linguistic: lexical, syntactic, factivity
- Logic: 
   - negation, boolean, quantifier, conditional, comparative, 
   - relational reasoning, spatial reasoning, temporal reasoning, causal reasoning, coreference reasoning
- Knowledge: world_knowledge, taxonomic_knowledge
- For Neutral Label: general_q2, subject_q2, object_q2

Apart from that, we also have the following columns:
- Premise and hypothesis: This is the same as the MultiNLI. They are repeated for the sake of completion.
- Label: Similar as MultiNLI
- Annotated Label: This is the label as predicted by our annotators.

These 18 binary features indicate whether a certain kind of reasoning capability is required to perform the inference for that example. 

## Files:
1. `taxinli10k.tsv` - This is the main TaxiNLI dataset file with 10071 annotated NLI examples. 
2. `taxinli10k_MNLIDev.tsv` - This is the part which overlaps with MultiNLI Dev dataset. We also include our Naive-Bayes, BERT and ESIM reults in the last three columns.

# TaxiNLI Statistics

Statistics |  |
--- | --- |
Total Datapoints | 10071 | 
Overlap with MNLI | 2343 (train), 7728 (dev) | 
Avg. Datapoints per Domain | 1007.1 | 
Datapoints per NLI label | 3374 (C), 3201 (N), 3494 (E) | 
Avg. Categories per example | 1.6 |
Neutral Example Stats | 3087 (Same topic), 2843 (Same object), 877 (Same subject)|


We also provide the statistics in the following figure grouper per category and label. 

![Alt text](category_plot_split.png?raw=true "Statistics of TaxiNLI Dataset")
 

# Contact

For any questions about the work, please contact Somak Aditya (t-soadit@microsoft.com).

# Citation

Kindly cite the CoNLL 2020 version:

```
@inproceedings{joshi-etal-2020-taxinli,
    title = "{T}axi{NLI}: Taking a Ride up the {NLU} Hill",
    author = "Joshi, Pratik  and
      Aditya, Somak  and
      Sathe, Aalok  and
      Choudhury, Monojit",
    booktitle = "Proceedings of the 24th Conference on Computational Natural Language Learning",
    month = nov,
    year = "2020",
    address = "Online",
    publisher = "Association for Computational Linguistics",
    url = "https://www.aclweb.org/anthology/2020.conll-1.4",
    pages = "41--55",
    abstract = "Pre-trained Transformer-based neural architectures have consistently achieved state-of-the-art performance in the Natural Language Inference (NLI) task. Since NLI examples encompass a variety of linguistic, logical, and reasoning phenomena, it remains unclear as to which specific concepts are learnt by the trained systems and where they can achieve strong generalization. To investigate this question, we propose a taxonomic hierarchy of categories that are relevant for the NLI task. We introduce TaxiNLI, a new dataset, that has 10k examples from the MNLI dataset with these taxonomic labels. Through various experiments on TaxiNLI, we observe that whereas for certain taxonomic categories SOTA neural models have achieved near perfect accuracies{---}a large jump over the previous models{---}some categories still remain difficult. Our work adds to the growing body of literature that shows the gaps in the current NLI systems and datasets through a systematic presentation and analysis of reasoning categories.",
}
```

# Contributing

This project welcomes contributions and suggestions.  Most contributions require you to agree to a
Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
the rights to use your contribution. For details, visit https://cla.opensource.microsoft.com.

When you submit a pull request, a CLA bot will automatically determine whether you need to provide
a CLA and decorate the PR appropriately (e.g., status check, comment). Simply follow the instructions
provided by the bot. You will only need to do this once across all repos using our CLA.

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or
contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.

# License and Legal Notice

We release the TaxiNLI dataset (and other data and code under https://github.com/microsoft/TaxiNLI) under the following Computational Use of Data Agreement ([LICENSE](https://github.com/microsoft/TaxiNLI/LICENSE)). By downloading this dataset and the contents, you are automatically agreeing to accept the use terms.
