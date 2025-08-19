# FastMCP requires Python 3.10 or newer
FROM python:3.13-slim

# Set the working directory in the container
WORKDIR /app

# Copy your FastMCP server code
COPY mcp_server.py /app/

# Copy your requirements.txt and install dependencies
COPY requirements.txt /app/
RUN pip install --no-cache-dir -r requirements.txt

# Expose the port the FastMCP server listens on (e.g., 8000)
EXPOSE 8000

# run FastMCP server
CMD ["python", "mcp_server.py"]
