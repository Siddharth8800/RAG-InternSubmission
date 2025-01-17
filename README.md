# RAG Chatbot

This repo contains the code for the submission and the jupyter notebook `working.ipynb` contains the code for generating the embeddings initially. The embedings are then saved in the `chroma_db` folder.

## Candidate Name: Siddharth

I have chosen to use Open source models instead of OpenAI API, beause it will give toy more control over the app + the cost savings.

### LLM Used: mistral-7b-instruct-v0.2.Q5_K_S.gguf

Although this model was not my first choice, it was originally Microsoft Phi-2 as it recently when open source, but in my testing mistral-7b-instruct-v0.2.Q5_K_S.gguf gave wayyyy better results and was more accurate.

### Embedding Model Used: BAAI/bge-large-en-v1.5

This model performs really high on the MTEB Leaderboard and is also open source, so I chose to use this model.

### How to run the code:

1. Clone the repo
2. Create a conda environment using the `requiremnets.txt` file
3. Use command `conda create -n newEnv --file requiremnets.txt`
4. Download the LLM model from [here](https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.2-GGUF/tree/main) and place it in the `same` folder.
5. Open the terminal and do `python app.py`

### My Hardware Specs:

1. CPU: Intel i7-13700K
2. GPU: Nvidia RTX 3090
3. RAM: 32GB G.Skill Ripjaws 6000mt/s

### Conclusion:

This took me wayy longer than expected beacuse I was having trouble deploying the app on HuggingFace Spaces, go I just went with locally hosting the app on my PC using Gradio Tunnel, I hope that's okay, but for future I'd rather just go with docker and not fiddle with HuggingFace Spaces.
