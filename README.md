bedrock-chatbot-project/
├── README.md                        # Overview, setup, architecture diagram
├── requirements.txt                 # Python dependencies for CDK and Lambdas
│
├── cdk/                             # CDK Infrastructure (Python)
│   ├── __init__.py
│   ├── app.py
│   ├── stack.py
│
│   ├── roles_policies/             # IAM roles & policies
│   │   └── roles.py
│
│   ├── knowledge_bases/
│   │   ├── documents_kb.py
│   │   ├── redshift_kb.py
│
│   ├── agents/
│   │   ├── document_agent.py
│   │   ├── redshift_agent.py
│
│   ├── guardrails/
│   │   └── guardrail_config.py
│
│   ├── api/
│   │   └── api_gateway.py
│
│   ├── lambdas/
│   │   ├── redshift_query/
│   │   │   └── handler.py
│   │   ├── summarizer/
│   │   │   └── handler.py
│   │   └── chat_handler/
│   │       └
