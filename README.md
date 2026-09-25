# MuleZero — Graph-Based Money-Mule Detection

A working FastAPI + NetworkX prototype that reconstructs transaction relationships as a directed money-flow graph and produces explainable risk signals.

## Run

```bash
pip install -r requirements.txt
uvicorn backend.app.main:app --reload
```

Open http://127.0.0.1:8000. Use `/api/demo/load` to load demo transactions and `/api/graph` to analyze them.

Run tests with `pytest`.

This is a synthetic-data hackathon prototype, not a production AML or banking decision system. The iNSIGHTS adapter is only an integration boundary until the official API/SDK details are available.
