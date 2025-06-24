FROM python:3.11-slim

# Install uv and dependencies
RUN pip install uv
WORKDIR /app
COPY . .

# Sync dependencies
RUN uv sync

EXPOSE 8002
CMD ["uv", "run", "app.py"]