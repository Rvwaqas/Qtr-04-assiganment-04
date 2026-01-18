FROM python:3.14-slim

WORKDIR /app

COPY . .

RUN pip install uv

RUN uv sync

EXPOSE 8000

CMD ["uv", "run", "main.py","--host","0.0.0.0","--port","8000"]