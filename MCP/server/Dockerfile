FROM python:3.13-slim

WORKDIR /app
COPY mcp_server.py /app/
COPY requirements.txt /app/
RUN pip install --no-cache-dir -r requirements.txt

EXPOSE 9001
CMD ["python", "mcp_server.py"]
