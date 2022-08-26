FROM python
WORKDIR /app
COPY requirements.txt .
RUN pip install -r requirements.txt
COPY . /app
CMD ["gunicorn", "--bind", "0.0.0.0:5000", "-c", "config.py", "app:app"]