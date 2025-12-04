elynt-ai/
│
├── config/
│   ├── agents.yaml          # Agent definitions (roles, goals, tools)
│   ├── tasks.yaml           # Task templates
│   ├── crew.yaml            # Crew definitions (pipelines)
│   ├── settings.yaml        # System/global config
│
├── src/
│   ├── main.py              # Entry point
│   ├── core/
│   │   ├── crew_loader.py   # Converts YAML → CrewAI objects
│   │   ├── agent_factory.py # Build agents dynamically
│   │   ├── task_factory.py  # Build tasks dynamically
│   │   ├── logger.py        # Custom logging
│   │   ├── errors.py        # Error handling
│   │
│   ├── agents/
│   │   ├── research_agent.py
│   │   ├── summarizer_agent.py
│   │   └── custom_agent.py
│   │
│   ├── tools/
│   │   ├── web_search.py
│   │   ├── file_tools.py
│   │   ├── rag_tool.py
│   │   └── browser_tool.py
│   │
│   ├── tasks/
│   │   ├── research_tasks.py
│   │   ├── summarization_tasks.py
│   │   └── custom_tasks.py
│   │
│   ├── pipelines/
│   │   ├── marketing_pipeline.py
│   │   ├── customer_support_pipeline.py
│   │   ├── analysis_pipeline.py
│   │   └── finance_agent_pipeline.py
│   │
│   ├── api/
│   │   ├── server.py        # FastAPI application
│   │   ├── routes/
│   │   │   ├── agents.py
│   │   │   ├── tasks.py
│   │   │   └── pipelines.py
│   │   ├── models/
│   │   │   ├── request_models.py
│   │   │   └── response_models.py
│   │
│   ├── services/
│   │   ├── agent_service.py # Call Crew via API
│   │   ├── pipeline_service.py
│   │   ├── rag_service.py
│   │   └── storage_service.py
│   │
│   ├── utils/
│   │   ├── env_loader.py
│   │   ├── helpers.py
│   │   ├── text_cleaner.py
│   │   └── jwt_auth.py
│
├── data/
│   ├── documents/           # RAG documents
│   ├── embeddings/          # Vector DB storage
│   └── knowledge_base/      # Static KB
│
├── tests/
│   ├── test_agents.py
│   ├── test_tools.py
│   ├── test_pipelines.py
│   └── test_api.py
│
├── docker/
│   ├── Dockerfile
│   ├── docker-compose.yaml
│
├── .env
├── requirements.txt
├── README.md
└── Makefile
