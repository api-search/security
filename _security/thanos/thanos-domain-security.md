---
api_specs:
- filename: thanos-query-api.yml
  format: yaml
  label: Thanos Query API
  slug: thanos-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thanos/refs/heads/main/openapi/thanos-query-api.yml
- filename: thanos-store-gateway-openapi.yml
  format: yaml
  label: Thanos Store Gateway API
  slug: thanos-store-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thanos/refs/heads/main/openapi/thanos-store-gateway-openapi.yml
- filename: thanos-sidecar-openapi.yml
  format: yaml
  label: Thanos Sidecar API
  slug: thanos-sidecar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thanos/refs/heads/main/openapi/thanos-sidecar-openapi.yml
- filename: thanos-ruler-openapi.yml
  format: yaml
  label: Thanos Ruler API
  slug: thanos-ruler-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thanos/refs/heads/main/openapi/thanos-ruler-openapi.yml
- filename: thanos-receive-openapi.yml
  format: yaml
  label: Thanos Receive API
  slug: thanos-receive-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thanos/refs/heads/main/openapi/thanos-receive-openapi.yml
- filename: thanos-compact-openapi.yml
  format: yaml
  label: Thanos Compact API
  slug: thanos-compact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thanos/refs/heads/main/openapi/thanos-compact-openapi.yml
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
