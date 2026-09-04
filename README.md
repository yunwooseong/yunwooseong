### Hi, I'm Woo-Seong Yun 👋

I build AI systems that uncover preferences users themselves may not yet recognize, focusing on making recommendations both accurate and explainable.

My research follows one principle: **rather than taking an observed failure at face value, find the structural cause behind it.** My M.S. thesis, *Two Contrastive Approaches for Addressing the Long-Tail Problem in Recommender Systems*, traced popularity bias hidden across model families from VAEs to LLMs, and the work since has kept digging beneath surface-level symptoms.

---

### 💼 Experience

**Machine Learning Engineer, [WATCHA](https://watcha.com)** · Dec 2025 – present

Personalized recommendation modeling and MLOps for webtoons, films and other content domains.

- **Recommendation modeling.** Analyze consumption patterns (viewing time, rating behavior, shifting genre preference) and turn them into personalization strategy; optimize collaborative filtering and ship new methods to production. Most recently, identified at the gradient level why popularity bias survives cosine-scored sampled softmax, designed a loss that removes it, and deployed it to in-house models (to appear at CIKM 2026).
- **LLM-based feature engineering.** Summarize large-scale review data with LLMs to feed models the concrete reasons behind a rating, not just the score.
- **A/B testing.** Design and run experiments on model changes and quantify impact on CTR, play rate and other KPIs to drive product decisions.

---

### 🎓 Education

- **M.S. in Artificial Intelligence** · Chung-Ang University (2023–2025)
- **B.S. in Applied Statistics** · Chung-Ang University (2018–2023)

---

### 📚 Publications

**Conference Papers**

- **[CIKM 2026, Co-first author]** Norm Removed, Bias Remains: Gradient-Decoupled Sampled Softmax for Collaborative Filtering. **WS Yun**\*, YJ Choi\*, YS Cho. [[Code]](https://github.com/yunwooseong/GD-SSM)
  Cosine scoring removes norms from the score, yet degree bias re-enters through per-update norm drift and per-epoch gradient accumulation. GD-SSM decouples both with an L2 projection and a closed-form degree prior, using a single hyperparameter. Validated on WATCHA production data.
- **[ICML 2026, Second author]** Capacity without Access: Reinterpreting the Mid-Depth Spectral Plateau in LLMs. SM Kang, **WS Yun**, N Lee, YS Cho. [[Paper]](https://openreview.net/forum?id=wsw7Y085RY) [[Code]](https://github.com/yunwooseong/Capacity-without-Access)
  Probing says deep layers grow richer; residual dynamics says they barely change. Separating representational *capacity* from readout *accessibility* shows mid-depth layers keep their spectral diversity but project weakly onto the output subspace. A diagnostic route (DDI) that exposes them to the readout improves 4 models on 12 benchmarks at zero inference cost, most on multi-step reasoning.
- **[WSDM 2026, First author]** ARROW: Adaptive Reasoning for LLM-based Recommendation with Explainability. **WS Yun**, MS Kim, YS Cho. [[Paper]](https://doi.org/10.1145/3773966.3779396) [[PDF]](https://drive.google.com/file/d/1w_3K_XB5Mp21gHbz7cys-RciBIzRzI5j/view?usp=drive_link) [[Code]](https://github.com/yunwooseong/ARROW)
  LLM recommenders could not explain their choices because of the semantic gap between linguistic knowledge and collaborative patterns. ARROW guides the LLM to infer latent tastes step by step and weights the reasoning loss by its own uncertainty, beating strong baselines while producing human-readable rationales.
- **[RecSys 2025, Co-first author]** Rethinking Overconfidence in VAEs: Can Label Smoothing Help? **WS Yun**\*, YJ Choi\*, YS Cho. [[Paper]](https://doi.org/10.1145/3705328.3748039) [[PDF]](https://drive.google.com/file/d/1efUR29wYnvczTYMfFP3xoDJadYDRquCZ/view?usp=drive_link) [[Code]](https://github.com/yunwooseong/RethinkVAE)
  Extreme sparsity and implicit feedback make VAE-based CF overconfident, and a gradient-level analysis shows this collapses embeddings into a low-rank subspace. Label smoothing restores the gradient, with the optimal factor decreasing as data get sparser.

**Journal Papers**

- **[Applied Soft Computing, Second author]** GCNs Meet Long-Tail: Embedding Norm Bias in GCN-Based Recommendations. YJ Choi, **WS Yun**, C Jeong, YS Cho. [[Paper]](https://doi.org/10.1016/j.asoc.2025.114226) [[PDF]](https://drive.google.com/file/d/1Hx8wZmoK_7J5Sr9Jz_lTNfEJtZAhlfya/view?usp=drive_link) [[Code]](https://github.com/yunwooseong/DNA)
  Popular items grow larger embedding norms under message passing. Analyzing that dynamic explains how long-tail bias forms, and a norm adjustment widens exposure for unpopular items.
- **[IEEE Access, Second author]** Enhancing LLMs for Sequential Recommendation with Reversed User History and User Embeddings. YJ Choi, **WS Yun**, YS Cho. [[Paper]](https://doi.org/10.1109/ACCESS.2025.3583094) [[PDF]](https://drive.google.com/file/d/17bjocYjYEQWBhESECv7iZsdhG9-gcggT/view?usp=drive_link) [[Code]](https://github.com/yunwooseong/LLM4Rec)
  Feeding history in order dilutes recent behavior across earlier tokens. Reversed history generation and a recency-weighted user embedding let recent interactions drive the prediction.
- **[IEEE Access, First author]** Contrastive Disentangled Variational Autoencoder for Collaborative Filtering. **WS Yun**, SM Kang, YS Cho. [[Paper]](https://doi.org/10.1109/ACCESS.2025.3576445) [[PDF]](https://drive.google.com/file/d/1sJxatVm-eE8VfrPVio5AKxaUkK8Vdnb3/view?usp=drive_link) [[Code]](https://github.com/yunwooseong/CD-VAE)
  Interactions mix genuine taste with popularity. Contrastive disentanglement against a popularity-based background separates the two and lifts recommendation quality on long-tail items.

**Under Review**

- **[Co-first author]** All Items are not Equal: Addressing the Imbalance of Item Knowledge in LLM for Recommendation.
  LLMs know items unevenly depending on pretraining exposure, and recommendation quality follows. Contrastive decoding at inference narrows the knowledge gap across items.
- **[Co-first author]** LINKER: Leveraging Modality Knowledge for Semantic Relation Generation in Multimodal Recommendation.
  Item modalities such as images and text are underused in multimodal recommendation. LINKER uses them to probabilistically generate interactions a user is likely to enjoy.

[→ Full publication list](https://yunwooseong.github.io/#publications)

---

### 📫 Contact

- **Email**: [dntjd0804@cau.ac.kr](mailto:dntjd0804@cau.ac.kr)
- **Website**: [yunwooseong.github.io](https://yunwooseong.github.io)
- **Google Scholar**: [Profile](https://scholar.google.com/citations?user=ZRXyvtMAAAAJ)
- **ORCID**: [0009-0002-2015-6566](https://orcid.org/0009-0002-2015-6566)
