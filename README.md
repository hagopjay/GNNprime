# GNNprime


🟢 Part 1 — Kindergarten cleans up and expands basic Data objects intro with a networkx visualisation of the cycle graph, attribute inspection, and a quick-reference table of the COO format.

🟡 Part 2 — Grade 5 refactors the NNConv node classifier with a fix to the label generation (now uses feature bucketing so the task is actually learnable), modular training utilities, gradient clipping, and a cosine LR scheduler with training curves.

🟠 Part 3 — Grade 10 rewrites EdgeAwareGAT cleanly, with an EarlyStop dataclass, proper AMP support, pre-norm residuals, and a side-by-side comparison table of upgrades vs Grade 5.

🔴 Part 4 — Real Datasets consolidates your scattered serialization-safety code into one clean _allowlist_pyg_classes() function, and fixes the locals()[name] bug (that pattern doesn't actually mutate local variables in Python — it silently does nothing).

🟣 Part 5 — Embeddings adds a embed() method shim to extract penultimate-layer representations, with both PCA and t-SNE visualisation.

⚫ Part 6 — Contrastive Pretraining unifies the scattered NT-Xent code, fixes the undefined cfg reference, and wraps everything in a clean pretrain_contrastive() function with both feature masking and edge dropout augmentations.

🖥️ Part 7 — GPU Monitoring consolidates all three monitoring cells with a threading.Event stop signal (cleaner than a global flag), and a post-run summary plot.
The notebook also includes a Summary table linking every part to the key PyG APIs, plus suggested next experiments (graph classification, link prediction, NeighborLoader, explainability).
