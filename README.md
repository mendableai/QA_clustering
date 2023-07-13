# Summarizing User Questions with LLMs

Question-Answering (QA) systems like Mendable have revolutionized the way users interact with technical documentation. They also could provide valuable insights to companies about what users are confused by and what are the common question themes.

However, discerning key themes from extensive sets of questions can be challenging. LLMs offer an innovative way to assist in question theme determination across large volumes of user queries.

We test `clustering` (group similar questions together followedf by LLM-assisted summary of themes per cluster) and `map-reduce` (breaking the questions down into smaller chunks, summarizing each, and then combining the results) to summarize question gathered from 1 month on the [LangChain documentation](https://python.langchain.com/docs/get_started/introduction.html).

Here is a summary of the approaches:

![summary](https://github.com/mendableai/QA_clustering/assets/122662504/2f6d4408-2eb3-49b1-92c6-5b2c4a2c7260)

See the two Jupyter notebooks in `notebooks`.

For LLMs used, you will need OpenAI and / or Anthropic API keys:
```
export OPENAI_KEY="your-api-key-here"
export ANTHROPIC_API_KEY="your-api-key-here"
```
Install packages and run:
```
cd notebooks
pip install -r requirements.txt
jupyter notebook
```

See related blog post [here](https://blog.langchain.dev/llms-to-improve-documentation/).
