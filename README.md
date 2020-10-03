# TaxiNLI

We release TaxiNLI dataset associated with [TaxiNLI: Taking a ride up the NLU Hill](https://arxiv.org/abs/2009.14505). Essentially each row in this data corresponds to an NLI example in the MultiNLI dataset (can be identified using pairID and genre). We add 18 features, namely:
- Linguistic: lexical, syntactic, factivity_linguistic
- Logic: negation, boolean, quantifier, conditional, comparative, relational reasoning, spatial reasoning, temporal reasoning, causal reasoning, coreference reasoning
- Knowledge: world_knowledge, taxonomic_knowledge
- For Neutral Label: general_q2, subject_q2, object_q2

Apart from that, we also have the following columns:
- Premise and hypothesis: This is the same as the MultiNLI. They are repeated for the sake of completion.
- Label: Similar as MultiNLI
- Annotated Label: This is the label as predicted by our annotators.

These 18 binary features indicate whether a certain kind of reasoning capability is required to perform the inference for that example. 

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
