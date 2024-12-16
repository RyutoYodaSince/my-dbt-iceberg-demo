FROM python:3.10-slim

# システム依存パッケージ(必要に応じて追加)
RUN apt-get update && apt-get install -y build-essential unixodbc-dev && rm -rf /var/lib/apt/lists/*

# dbt & athena adapterインストール
RUN pip install --no-cache-dir dbt-athena-adapter[athena]

WORKDIR /usr/app
