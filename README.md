# self_RAG

Self-RAG is a new framework to train an arbitrary LM to learn to retrieve, generate, and critique to enhance the factuality and quality of generations, without hurting the versatility of LLMs.

Unlike a widely-adopted Retrieval-Augmented Generation (RAG; Figure left) approach, Self-RAG retrieves on demand (e.g., can retrieve multiple times or completely skip retrieval) given diverse queries, and criticize its own generation from multiple fine-grained aspects by predicting reflection tokens as an integral part of generation. We conduct a segment-wise beam search to select the output that maximizes the utility for diverse preferences.
