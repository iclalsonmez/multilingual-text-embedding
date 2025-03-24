# multilingual-text-embedding
This repository contains an analysis and comparison of various multilingual text embedding models and the 'ytu-ce-cosmos/turkish-colbert' model. These models are evaluated with respect to their architecture, parameter sizes, and potential use cases in NLP tasks and visualized with t-SNE.

Models Included
The following text embedding models are examined:

IBM Granite Embedding 107M (ibm-granite/granite-embedding-107m-multilingual)
Multilingual text embedding model
107 million parameters
Developed by IBM

Alibaba GTE Multilingual Base (Alibaba-NLP/gte-multilingual-base)
Multilingual text embedding model
108 million parameters
Developed by Alibaba

YTU Turkish ColBERT (ytu-ce-cosmos/turkish-colbert)
Optimized for the Turkish language
Based on the ColBERT architecture
Developed by Yildiz Technical University

Multilingual E5 Small (intfloat/multilingual-e5-small)
Multilingual embedding model
118 million parameters
Part of the E5 model series

Paraphrase Multilingual MiniLM-L12-v2 (sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2)
118 million parameters
Uses the MiniLM architecture
Optimized for paraphrase detection

Paraphrase Multilingual MPNet Base-v2 (sentence-transformers/paraphrase-multilingual-mpnet-base-v2)
Multilingual text embedding model
Uses MPNet architecture
Optimized for semantic similarity and ranking tasks

-------------------------------------------------------------------------------------------------
To explore and evaluate these models, you can use the Hugging Face sentence-transformers library:

from sentence_transformers import SentenceTransformer

model_name = "sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2"
model = SentenceTransformer(model_name)

sentence = "This is a test sentence."
embedding = model.encode(sentence)
print(embedding)
