# DataPlatform_DE25_Rikard_Oledal_Lecture5
DataPlatform course at STI

## Storing data - philosophy

* What's the purpose of our data?
    * Bulk uploading
    * JSON data storage

- fastapi dev main.py

```postgresql
CREATE TABLE IF NOT EXISTS products_raw (
id BIGSERIAL PRIMARY KEY,
created_at TIMESTAMPTZ NOT NULL DEFAULT now(),
product JSONB NOT NULL
);
```