# code-cracker-lib
Code base cracker library provides code cracker a powerful backend Python library

python package(will publish to https://packaging.python.org/en/latest/tutorials/packaging-projects/) 

Keywords: **Large Language Model(LLM) + Knowledge Extraction(KG)**

The library will contains all functions for the following workflow.

## Knowledge extraction

<aside>
💡 Code-base simplification workflow

1. Meta-knowledge extraction
    - git commit history extraction
    - code dependency extraction
2. Knowledge graphs extraction ← (meta-knowledge, and code-base) [code KG, learn KG]
    - code KG is a knowledge graph based on code-base and their meta-knowledge
    - learn KG is a knowledge graph based on external material such as books for users to have more insights on code-base.
3. Create simplification variants KG
</aside>

## Knowledge application

<aside>
💡 QA workflow

1. Create idea/question [data source: simplified code KG, learn KG]
2. Create summarized answer [data source: simplified code KG, learn KG]
3. Find reference [data source: simplified code KG, learn KG]
</aside>

<aside>
💡 Code Injection workflow [Target language: Python / JS / TS]

1. Create Motivation / Prompted with motivation [data source: common motivation + code KG] 
2. Get test-bed
3. Generate tests
4. Run tests
5. Iterative improve tests
</aside>

## Knowledge update

<aside>
💡 Code-base simplification enhanced workflow

1. Human-label extraction
2. Knowledge graph update ← (data source: simplified code KG, learn KG and user interaction trace)
</aside>

## Knowledge Storage Format

<aside>
💽 Different storage formats for knowledge graphs

- Node
    - reference
    - knowledge
    - link
    
- Reference
    - type
    - file path
    - content
    
- Knowledge
    - type
    - content
    
- link
    - type
    - src_node
    - dest_node
    
</aside>
