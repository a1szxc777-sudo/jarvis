FROM python:3.12-slim
ENV PYTHONUNBUFFERED=1 TZ=Asia/Almaty DATA_DIR=/data
WORKDIR /app
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt
COPY bot.py .
VOLUME /data
CMD ["python", "bot.py"]
