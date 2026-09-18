FROM python:3.11-slim

WORKDIR /app

RUN pip install --no-cache-dir mem0-open-mcp

# mem0-open-mcp looks for mem0-open-mcp.yaml in its working directory
COPY mem0-open-mcp.yaml .

EXPOSE 8765

CMD ["mem0-open-mcp", "serve", "--port", "8765"]
