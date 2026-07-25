---
api_key_in: []
api_specs:
- filename: prometheus-admin-api-openapi.yml
  format: yaml
  label: Prometheus Admin API
  slug: prometheus-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometheus/refs/heads/main/openapi/prometheus-admin-api-openapi.yml
- filename: prometheus-alerts-api-openapi.yml
  format: yaml
  label: Prometheus Alerts API
  slug: prometheus-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometheus/refs/heads/main/openapi/prometheus-alerts-api-openapi.yml
- filename: prometheus-lifecycle-api-openapi.yml
  format: yaml
  label: Prometheus Lifecycle API
  slug: prometheus-lifecycle-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometheus/refs/heads/main/openapi/prometheus-lifecycle-api-openapi.yml
- filename: prometheus-metadata-api-openapi.yml
  format: yaml
  label: Prometheus Metadata API
  slug: prometheus-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometheus/refs/heads/main/openapi/prometheus-metadata-api-openapi.yml
- filename: prometheus-metrics-api-openapi.yml
  format: yaml
  label: Prometheus Metrics API
  slug: prometheus-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometheus/refs/heads/main/openapi/prometheus-metrics-api-openapi.yml
- filename: prometheus-query-api-openapi.yml
  format: yaml
  label: Prometheus Query API
  slug: prometheus-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometheus/refs/heads/main/openapi/prometheus-query-api-openapi.yml
- filename: prometheus-receivers-api-openapi.yml
  format: yaml
  label: Prometheus Receivers API
  slug: prometheus-receivers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometheus/refs/heads/main/openapi/prometheus-receivers-api-openapi.yml
- filename: prometheus-rules-api-openapi.yml
  format: yaml
  label: Prometheus Rules API
  slug: prometheus-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometheus/refs/heads/main/openapi/prometheus-rules-api-openapi.yml
- filename: prometheus-silences-api-openapi.yml
  format: yaml
  label: Prometheus Silences API
  slug: prometheus-silences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometheus/refs/heads/main/openapi/prometheus-silences-api-openapi.yml
- filename: prometheus-status-api-openapi.yml
  format: yaml
  label: Prometheus Status API
  slug: prometheus-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometheus/refs/heads/main/openapi/prometheus-status-api-openapi.yml
- filename: prometheus-targets-api-openapi.yml
  format: yaml
  label: Prometheus Targets API
  slug: prometheus-targets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometheus/refs/heads/main/openapi/prometheus-targets-api-openapi.yml
- filename: prometheus-tsdb-api-openapi.yml
  format: yaml
  label: Prometheus TSDB API
  slug: prometheus-tsdb-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometheus/refs/heads/main/openapi/prometheus-tsdb-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Prometheus Authentication
name_suffix: Authentication
oauth_flows: []
overview: Prometheus declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Prometheus
provider_slug: prometheus
scheme_count: 0
schemes: []
slug: prometheus-authentication
source_filename: prometheus-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-06-20'\nmethod: searched\nsource: https://prometheus.io/docs/guides/basic-auth/, https://prometheus.io/docs/prometheus/latest/querying/api/\ndocs: https://prometheus.io/docs/guides/basic-auth/\nsummary:\n  types: []\n  api_key_in: []\n  oauth2_flows: []\n  built_in_auth: false\nmodel: >-\n  Prometheus, Pushgateway, and Alertmanager ship with NO built-in application-level\n  authentication or authorization on their HTTP APIs. None of the OpenAPI specs declare a\n  securityScheme. Access control is expected to be provided externally.\nmechanisms:\n  - name: web-config-basic-auth\n    description: >-\n      Since 2.24.0 the server supports TLS and HTTP Basic Auth via a --web.config.file\n      (web-config.yml) with bcrypt-hashed basic_auth_users. This secures the server's own\n      endpoints without a proxy.\n    docs: https://prometheus.io/docs/guides/basic-auth/\n    optional: true\n  - name: web-config-tls\n    description: TLS server certificates and optional\
  \ mTLS client auth configured via --web.config.file.\n    docs: https://prometheus.io/docs/prometheus/latest/configuration/https/\n    optional: true\n  - name: reverse-proxy\n    description: >-\n      The canonical pattern for authenticated/authorized/multi-tenant access is to front\n      Prometheus with a reverse proxy (nginx, OAuth2 Proxy, service mesh) that enforces\n      OAuth/OIDC/SSO and network policy.\n    docs: https://prometheus.io/docs/operating/security/\n    optional: true\n  - name: admin-flags\n    description: >-\n      Destructive/administrative endpoints are gated by server flags rather than tokens —\n      --web.enable-lifecycle (config reload, quit) and --web.enable-admin-api (TSDB\n      snapshot, delete series, clean tombstones). Disabled by default.\n    docs: https://prometheus.io/docs/prometheus/latest/management_api/\n    optional: false\nschemes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prometheus/refs/heads/main/authentication/prometheus-authentication.yml
summary_line: 0 schemes
tags:
- Alerting
- Metrics
- Monitoring
- Observability
- Time Series
---
