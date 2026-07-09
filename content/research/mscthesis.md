---
title: "Structural Representation Learning and the Characterisation and Interpretation of Latent Manifolds — A Group-Theoretic Approach"
date: 2026-07-09T16:12:00+02:00
draft: false
description: "Masters Thesis"
image: "/images/cover_page.png"
tags: ["Machine Learning", "Group Representation Theory"]
repo: "" 
link: "" 
---
# Abstact:

Capturing the intrinsic structural relations of data is crucial for the generalisation and interpretability of neural networks. Group theory provides the foundational algebraic framework to rigorously define and embed these structural priors into machine learning models. While existing group-theoretic architectures, such as group-equivariant networks, successfully encode these relations, they lack semantically interpretable latent spaces. Conversely, group-homomorphism networks provide an interpretable latent space; however, they require explicit structural supervision or the hardcoding of algebraic structures within the latent space, limiting their real-world applicability.

To address these limitations, we formalise the class-aware and class-agnostic structural relations of data as abstract group actions. Building upon this, we introduce a scalable framework for implicit learning and the rigorous interpretation of these relations within latent spaces of neural networks. Our weakly supervised approach pairs an equivariant autoencoder with a learnable group representation approximator. During training, randomly sampled data pairs are passed through the autoencoder; at each forward pass, the approximator acts as a homomorphism, conditioning the latent space to preserve structural properties using only the resulting pairs of latent embeddings. The autoencoder and the approximator are trained jointly without requiring explicit structural supervision. Under this formulation, we mathematically prove that the approximator converges to a faithful representation for both finite discrete and compact Lie groups.

Furthermore, we explicitly characterise the latent space topology as smooth manifolds within the General Linear Group or the combined Radial Scaling and Orthogonal Group. By leveraging the direct correspondence between Lie algebras and their associated groups, we provide a mathematically grounded method for interpreting encoded relations within the latent space via exact manifold traversal. We show a strong correspondence between our empirical results and theoretical foundations throughout our experiments and ablations, demonstrating that our framework faithfully and implicitly uncovers structural relations within the latent space across both class-aware and class-agnostic regimes.

In summary, this work provides a group-theoretic formulation of the structural relations of data, alongside a framework to faithfully learn these relations within the latent space in the absence of explicit relational annotations. Importantly, it establishes a rigorous group-theoretic interpretation of latent space topology, allowing these relations to be inspected. That said, the framework's efficacy on downstream machine learning tasks remains to be examined.