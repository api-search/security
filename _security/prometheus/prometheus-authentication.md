---
api_key_in: []
api_specs:
- filename: prometheus-http-api-openapi.yml
  format: yaml
  label: Prometheus HTTP API
  slug: prometheus-http-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometheus/refs/heads/main/openapi/prometheus-http-api-openapi.yml
- filename: prometheus-management-api-openapi.yml
  format: yaml
  label: Prometheus Management API
  slug: prometheus-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometheus/refs/heads/main/openapi/prometheus-management-api-openapi.yml
- filename: prometheus-pushgateway-api-openapi.yml
  format: yaml
  label: Prometheus Pushgateway API
  slug: prometheus-pushgateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometheus/refs/heads/main/openapi/prometheus-pushgateway-api-openapi.yml
- filename: prometheus-alertmanager-api-openapi.yml
  format: yaml
  label: Prometheus Alertmanager API
  slug: prometheus-alertmanager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometheus/refs/heads/main/openapi/prometheus-alertmanager-api-openapi.yml
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
