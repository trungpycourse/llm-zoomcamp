

def rag(query):
    search_results = search(query)
    prompt = build_prompt(query, search_results)
    answer = llm(prompt)
    return answer

Ở trên là qui trình RAG
trong course này sẽ cover từng sections sau:
1. RAG flow
2. replace OpenAI  to Ollama
3. vector search , evaluating seach engine  
4. evaluating rag 


module 1: 

evaluating retrieval

- hitrate
- mrr 

evaluation 

- offline evaluation
    - cosine similarity
    - LLM-as-a-judge

ground truth dataset
answer_original -> question -> answer_llm
cosine(answer_original, answer_llm)
llm_as_a_judge(answer_original, answer_llm)
llm_as_a_judge(question, answer_llm)

- online evaluation
    - AB tests, experiments
    - user feedback

- monitoring
    - overall health of the system 