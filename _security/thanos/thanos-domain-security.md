---
api_specs:
- filename: thanos-alerts-api-openapi.yml
  format: yaml
  label: Thanos Alerts API
  slug: thanos-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thanos/refs/heads/main/openapi/thanos-alerts-api-openapi.yml
- filename: thanos-blocks-api-openapi.yml
  format: yaml
  label: Thanos Blocks API
  slug: thanos-blocks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thanos/refs/heads/main/openapi/thanos-blocks-api-openapi.yml
- filename: thanos-health-api-openapi.yml
  format: yaml
  label: Thanos Health API
  slug: thanos-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thanos/refs/heads/main/openapi/thanos-health-api-openapi.yml
- filename: thanos-metadata-api-openapi.yml
  format: yaml
  label: Thanos Metadata API
  slug: thanos-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thanos/refs/heads/main/openapi/thanos-metadata-api-openapi.yml
- filename: thanos-metrics-api-openapi.yml
  format: yaml
  label: Thanos Metrics API
  slug: thanos-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thanos/refs/heads/main/openapi/thanos-metrics-api-openapi.yml
- filename: thanos-query-api-openapi.yml
  format: yaml
  label: Thanos Query API
  slug: thanos-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thanos/refs/heads/main/openapi/thanos-query-api-openapi.yml
- filename: thanos-remote-write-api-openapi.yml
  format: yaml
  label: Thanos Remote Write API
  slug: thanos-remote-write-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thanos/refs/heads/main/openapi/thanos-remote-write-api-openapi.yml
- filename: thanos-rules-api-openapi.yml
  format: yaml
  label: Thanos Rules API
  slug: thanos-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thanos/refs/heads/main/openapi/thanos-rules-api-openapi.yml
- filename: thanos-stores-api-openapi.yml
  format: yaml
  label: Thanos Stores API
  slug: thanos-stores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thanos/refs/heads/main/openapi/thanos-stores-api-openapi.yml
- filename: thanos-targets-api-openapi.yml
  format: yaml
  label: Thanos Targets API
  slug: thanos-targets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thanos/refs/heads/main/openapi/thanos-targets-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: thanos.io
  spf: false
hosts:
- cert_expires: Aug 18 00:23:56 2026 GMT
  host: thanos.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Thanos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Thanos, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Thanos
provider_slug: thanos
slug: thanos-domain-security
source_filename: thanos-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: thanos.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 00:23:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: thanos.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thanos/refs/heads/main/security/thanos-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Metrics
- Monitoring
- Observability
- Prometheus
- Time Series Database
---
