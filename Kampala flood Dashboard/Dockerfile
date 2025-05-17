FROM python:3.10-slim
RUN apt-get update && apt-get install -y libgeos-dev proj-bin
COPY requirements.txt .
RUN pip install -r requirements.txt
COPY . .
CMD ["streamlit", "run", "app.py"]
