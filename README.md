# IR-Superproject-2023

The integration of large language models such as BERT, GPT, and ChatGPT into search engine applications is revolutionizing the way we search for information. This themed project aims to help you understand, engage with, and advance this technology.

Through this project, you will develop an in-depth understanding of these language models and their applications in powering search engines. You will have the opportunity to explore one of several research directions that we have identified. For instance, you may choose to investigate the effectiveness of these methods under specific conditions, such as studying possible biases and robustness issues, or you design, develop, and evaluate new solutions to address known problems that affect these methods.

While completion of the INFS7410 course at UQ, or a similar Information Retrieval and Web Search course at other universities is desirable, we will provide background information and study material in the initial weeks of the project to allow you to explore these methods in depth. Therefore, if you possess a strong understanding of key artificial intelligence concepts but lack specific information retrieval knowledge, you're still encouraged to undertake this project.


## Background material and videos

Links to videos:

- [BERT](https://youtu.be/pkHVCi973Wk)
- [BERT For Ranking](https://youtu.be/9sf9OCEHISI)
- [BERT Limitations](https://youtu.be/eamJUeYKUoY)
- [Handling Length by Scores](https://youtu.be/WgAwAqyERVs)
- [Handling Length by Representations with PARADE](https://youtu.be/9LZUL5M5cdI)
- [duoBERT](https://youtu.be/MuPWwAKPNVY)
- [doc2query](https://youtu.be/pJWK6DztaZg)
- [DPR](https://youtu.be/qLWa4pxfsiU)
- [ANCE](https://youtu.be/mT-I9DMiMRo)
- [RepBERT](https://youtu.be/AKpg3FVUTD8)
- [CLEAR](https://youtu.be/OB87Af3PPK8)
- [EPIC](https://youtu.be/6YNldDe1dBk)
- [DRs Performance](https://youtu.be/oMCJDBs81Og)
- [TILDE](https://youtu.be/BZCkf2QV07Q)
- [TILDEv2](https://youtu.be/BSxqIPeeLrU)

Readings:

- [Tonellotto, N., 2022. Lecture Notes on Neural Information Retrieval. arXiv preprint arXiv:2207.13443.](https://arxiv.org/pdf/2207.13443.pdf)
- [Zhao, W.X., Liu, J., Ren, R. and Wen, J.R., 2022. Dense text retrieval based on pretrained language models: A survey. arXiv preprint arXiv:2211.14876.](https://arxiv.org/pdf/2211.14876)



## Project Directions

1. Reproduce the paper [Penha, G., Câmara, A. and Hauff, C., 2022, April. Evaluating the robustness of retrieval pipelines with query variation generators. In Advances in Information Retrieval: 44th European Conference on IR Research, ECIR 2022, Stavanger, Norway, April 10–14, 2022, Proceedings, Part I (pp. 397-412). Cham: Springer International Publishing.](https://arxiv.org/pdf/2111.13057).

2. Reproduce the paper [Chen, X., Luo, J., He, B., Sun, L., and Sun, Y., 2023. Towards Robust Dense Retrieval via Local Ranking Alignment. Proceedings of the Thirty-First International Joint Conference on Artificial Intelligence (IJCAI-22)](https://www.ijcai.org/proceedings/2022/0275.pdf).

3. Reproduce the paper [Wu, C., Zhang, R., Guo, J., Fan, Y. and Cheng, X., 2022. Are neural ranking models robust?. ACM Transactions on Information Systems, 41(2), pp.1-36.](https://dl.acm.org/doi/pdf/10.1145/3534928).

4. Pre-trained Language Models-based rankers for Product Search. You will work with the [Amazon Shopping Queries Dataset](https://arxiv.org/abs/2206.06588), which is [publicly available](https://github.com/amazon-science/esci-data). Multiple directions here:
    - Query Generation. In product search, rankers are very effective if they model user behaviour; however new products will not have behavioural features, importantly they will not have relevant queries associated. You will be setting up a ranking pipeline (to different level of complexity) and implement query generation methods
    - Neural features such those generated from cross-encoder rankers have been shown very effective when used in a learning to rank pipeline for product search (e.g. based on [gradient boosted tree](https://link.springer.com/article/10.1007/s10791-009-9112-1)). However, cross-encoder features are expensive to generate and can only be generated for historic queries, i.e. queries observed in a query log -- i.e. offline (not real time). In this direction you will study the effect non generating cross-encoder features have on the rankers, and will investigate the effectiveness of weaker but computationally feasible neaural features, e.g. those generated by bi-encoders (dense retrievers). 

5. Participate in a TREC competition (only available for students with GPA >= 6). This includes all aspects of the competition, including creation of the pipeline, baselines, implementation of our methods, result analysis. Competition of interest:
    - [TREC Product Search](https://trec-product-search.github.io/): This competition uses the Amazon Shopping Queries Dataset](https://arxiv.org/abs/2206.06588), which is [publicly available](https://github.com/amazon-science/esci-data). Task 1 (Product Ranking Task): The first task focuses on product ranking. In task we provide an initial ranking of 100 documents from a BM25 baseline and you are expected to re-rank the products in terms of their relevance to the users given intent. The ranking provides a focused task where the candidate sets are fixed and there is no need to implement complex end to end systems which makes experimentation quick and runs easily comparable. Task 2 (Product Retrieval Task): The second task focuses on end to end product retrieval. In task we provide an a large collection of products and participants need to design end to end retrieval systems which leverage whichever information they find relevant/useful. Unlike the ranking task, the focus here is in understanding the interplay between retrieval and reranking systems.
    - [NeuCLIR Track](https://neuclir.github.io/): The track is focused on the application of modern neural computing techniques to cross-language information retrieval. NeuCLIR topics are written in English. NeuCLIR has three target language collections in Chinese, Persian, and Russian.



## Activities

* Week 5: [Video: Welcome and Project Proposal Draft Assessment](https://youtu.be/fc0MYSQg1EQ)




## Useful Links

- [ITEE Project Database](https://student.eait.uq.edu.au/projects/)
- [Ask questions and see answers through the GitHub issues](https://github.com/ielab/IR-Superproject-2023/issues?q=)
