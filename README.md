# langchain
## I have used langchain with OpenAI api to tackle the token limit problem and successfully created a personalized assistant for a custom dataset

In the jupyter notebook **langchain_git**, this code trains the LLM on any github repository, this can be really helpful when the github repo contains 
documentations for a particular framework not already trained by the OpenAI model, especially when the commit is made after Nov 2021. This may be 
used to train or guide users to navigate a new and daunting framework, and since it's not pragmatic to upload each file to ChatGPT.

In the jupyter notebook **langchain_aries**, I have used the code from **langchain_git** to train the model on the Hyperledger Aries Cloud Agent Python 
framework. The hyperledger aries is a breakthrough technology in using Zero Knowledge Proofs, for creating accessible Decentralized Identifiers (DIDs)
a big use case is credential verification without having to reveal personal info. Now major commits have been made in this repo in 2022, so the model has
 not been trained on this. After training 
the LLM on this repo, the model can practically teach me the entire working, architecture, code and application of the Hyperledger aries. Also, one 
additional feature I only came to know after using the assistant is that it can explain to me the importance and integration of certain files that are
not mentioned in the documentation.

In the jupyter notebook **langchain_pdf**, I took a different and a slightly more efficient method to solve a similar problem, to input large pdfs,
essentially large books and or research papers. I have used a cloud vector database called **Pinecone**. For one, this can be really cost effective as you
wouldn't have to make multiple api calls and the second benefit is that we can have more than one book, and different forms of text data. This could be a 
large dataset, and we could potentially fine tune the model to become an expert on the field of study.

My next goal would be to try and make a stack helper application, that uses langchain agents or agent executors to link multiple tools and sequence
chains that span over a large database containing text docs,github repos,google meet transcripts, sql databases and various API access and integrate 
it into the LLM, this model would be an expert on the stack and we would just have to guide the model into the direction we desire to take.

P.S. I understand that people are concerned about the fact that, as developers we might become completely dependant on the use of AI. But, similar to 
Google or Stackoverflow it is just a really good tool that increases our productivity, so that we can focus on more creative side problems. And, given 
the advancements we have seen this year with LLMs, it would be stupid not to use it. That said, I wish to familiarize myself with all the open source 
tools and frameworks in this field, and solve more problems.
