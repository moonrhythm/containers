FROM wrouesnel/postgres_exporter:v0.5.1

env PG_EXPORTER_EXTEND_QUERY_PATH=/config/queries.yaml
env PG_EXPORTER_AUTO_DISCOVER_DATABASES=true
env PG_EXPORTER_DISABLE_DEFAULT_METRICS=true
env PG_EXPORTER_DISABLE_SETTINGS_METRICS=true

COPY queries.yaml /config/queries.yaml
