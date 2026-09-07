---
api_specs:
- filename: corva-ai-platform-api-openapi.yml
  format: yaml
  label: Corva Platform API
  slug: corva-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/corva-ai/refs/heads/main/openapi/corva-ai-platform-api-openapi.yml
- filename: corva-ai-data-api-openapi.yml
  format: yaml
  label: Corva Data API
  slug: corva-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/corva-ai/refs/heads/main/openapi/corva-ai-data-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: corva.ai
  spf: true
hosts:
- cert_expires: Nov 30 04:01:47 2026 GMT
  host: www.corva.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 23 23:59:59 2027 GMT
  host: api.corva.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 20 23:59:59 2027 GMT
  host: dc-docs.corva.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Corva Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Corva AI, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Corva AI
provider_slug: corva-ai
slug: corva-ai-domain-security
source_filename: corva-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.corva.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 04:01:47 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.corva.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 23 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: dc-docs.corva.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 20 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: corva.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/corva-ai/refs/heads/main/security/corva-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Analytics
- Artificial Intelligence
- Completions
- Custom Apps
- Data API
- Dev Center
- Dev Center Apps
- Drilling
- Energy
- Geoscience
- Oil and Gas
- Platform API
- Predictive Drilling
- Python SDK
- Real-Time
- Real-Time Analytics
- Sensor Data
- Sustainability
- Time Series
- WITS
- Well Data
---
