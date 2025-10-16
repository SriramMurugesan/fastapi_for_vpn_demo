# fastapi_for_vpn_demo

## Setup

```bash
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

## Running locally

```bash
uvicorn app.main:app --reload
```

Visit `http://127.0.0.1:8000` to see the default response and `http://127.0.0.1:8000/docs` for interactive API docs.

## Docker

Build the image:

```bash
docker build -t fastapi_vpn_demo .
```

Run the container:

```bash
docker run -d --name fastapi_vpn_demo -p 8000:80 fastapi_vpn_demo
```

Navigate to `http://localhost:8000` to test.

## Project structure

```
fastapi_for_vpn_demo/
├── app/
│   └── main.py
├── requirements.txt
└── README.md
```