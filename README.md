# Large Language Models (LLMs)

Go through all main components of a LLMs system from scratch:
1. **Main components overview** (at LLMs_sys_summary.ipynb)
2. **Retrieval-Augmented Generation** (RAG):

Create RAG application for question answering over a document. These include extracting information, retrieving the relevant context, and utilizing this context to generate accurate results.

<img src="https://miro.medium.com/v2/resize:fit:1100/format:webp/0*hikPIs0EQ1CJ4qrz" alt="My Image" width="500">
Step 1: extract information from this document.

Step 2: break the document into smaller chunks, to fit into LLM context windows.

Step 3: two strategies to save documents for future retrieval:
- store the text as-is for keyword based retrieval.
- convert text into vector embeddings, for more efficient retrieval.

Step 4: save this to a relevant database.

Step 5: obtain relevant chunks based on user inputs.

Step 6: incorporate relevant document chunks as part of LLM context, for generating the output.

3. **Chain of Thought (CoT)**

CoT prompting in NLP used to guide the responses generated by language models, often improves interpretability and accuracy for more complex queries.

4. **Building a Llama 3 model** step by step
<img src='https://miro.medium.com/v2/resize:fit:1100/format:webp/1*_xNP7aBpcmcMk4tXJ-Z8Mw.png' width='400'>

- The Input Block with Byte Pair Encoding (BPE) tokenizer.
- The Decoder Block with sub-components:
  - RMS Norm (Root Mean Square Normalization)
  - RoPE (Rotary Positional Encoding)
  - KV Cache
  - Group Query Attention
  - FeedForward Network
- The Output Block.
