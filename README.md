# 기초부터 심화까지 RAG 쿡북 with Python

LLM 구축을 위한 RAG 기초부터 심화까지 21개의 방법론 실전 가이드

## 책 소개

이 책이 포함된 LLM Master 시리즈는 생성형 AI 시대를 살아가는 실무자와 개발자를 위해 기획되었다. ChatGPT를 비롯한 다양한 AI 도구들이 우리 일상과 업무에 빠르게 스며들고 있지만, 단순한 활용을 넘어 AI를 ‘내 일’과 ‘내 프로젝트’에 제대로 접목시키는 사람은 아직 많지 않다. LLM Master 시리즈는 이러한 격차를 줄이기 위해, 기초 이론부터 실무 프로젝트에 이르기까지 LLM을 완전히 내재화할 수 있는 커리큘럼을 제공한다. 특히 Python을 기반으로 한 코딩 중심 구성으로, 독자 스스로 AI 기능을 직접 구현하고 테스트하며 체화할 수 있도록 돕는다.

LLM(Large Language Model)을 구현하기 위한 프레임워크는 목적과 활용 환경에 따라 매우 다양하다.

우선, OpenAI, Claude(Anthropic), Grok(X), DeepSeek 등에서 제공하는 상용 LLM API를 단순히 호출하여 사용하는 경우에는, Python의 openai 라이브러리나 해당 서비스에서 제공하는 공식 SDK만으로도 충분히 구현할 수 있다. 이 방식은 상대적으로 설정이 간단하며, 모델을 별도로 구축하지 않아도 강력한 LLM 기능을 빠르게 활용할 수 있다는 장점이 있다.

하지만 단순한 LLM 호출을 넘어, 문서 기반 검색 및 생성(RAG, Retrieval-Augmented Generation)과 같은 고급 기능을 구현하려면 다양한 컴포넌트를 함께 조합해야 한다. 이럴 때는 다음과 같은 LLM 개발 전용 프레임워크를 활용하는 것이 효율적이다:

- LangChain은 LLM 기반 워크플로우를 구성하는 데 특화된 프레임워크로, 프롬프트 작성, 체인 구성, 툴 연동, 메모리 관리 등 다양한 기능을 제공한다.
    
- LlamaIndex는 문서 기반 검색에 특화되어 있으며, 문서를 효율적으로 인덱싱하고 검색 결과를 LLM에 전달하기 위한 구조를 갖추고 있다.
    
- Vector Store 라이브러리로는 FAISS, Chroma, Weaviate 등이 있으며, 임베딩 기반 검색 기능을 구현할 수 있다.
    
- 다양한 외부 도구를 LLM과 함께 연동하여 사용할 수 있는 Tool 구성 요소도 함께 활용할 수 있다.
    

상용 API가 아닌 오픈소스 LLM 모델을 직접 운영하거나 파인튜닝하고자 한다면, Hugging Face의 Transformers, accelerate, datasets, PEFT 등의 생태계를 활용하는 것을 권장한다. 이 경우에도 LangChain이나 LlamaIndex는 전처리, 검색, 체인 연결 등에 유용하게 활용할 수 있다. 오픈소스 모델은 로컬 또는 프라이빗 서버 환경에서 운영이 가능하다는 점에서 민감한 데이터를 다룰 때 특히 유리하다.

## 목 차

저자 소개.

Table of Contents

0장. RAG를 시작하기 전에.

1장. 기본 RAG: Simple RAG

2장. 시만틱 청킹: Semantic Chunking

3장. 청크 사이즈: Chunk Sizes RAG

4장. 문맥 강화: Context-Enriched RAG

5장. 헤드 추출: Contextual Chunk Headers

6장. 문서 증강: Document Augmentation RAG

7장. 쿼리 전환: Query Transformation RAG

8장. Reranking RAG

9장. RSE: Relevant Segment Extraction RAG

10장. 문맥 압축: Contextual Compression RAG

11장. 피드백 루프: Feedback Loop RAG

12장. 적응형 검색: Adaptive Retrieval RAG

13장. Self-RAG

14장. 명제 청킹: Proposition Chunking RAG

15장. 멀티모달: Multi-Modal RAG

16장. Fusion Retrieval RAG

17장. 그래프: Graph RAG

18장. 계층적 색인: Hierarchical Indices RAG

19장. HyDE

20장. CRAG: Corrective RAG

21장. 강화학습: RL with RAG

References. 참고 문헌

## E-Book 구매

## Github 코드

[https://github.com/no-wave/book-llm-master-rag-techniques](https://github.com/no-wave/book-llm-master-rag-techniques)
