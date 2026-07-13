---
api_specs:
- filename: refuel-ai-openapi.yml
  format: yaml
  label: Refuel Applications API
  slug: refuel-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/refuel-ai/refs/heads/main/openapi/refuel-ai-openapi.yml
- filename: refuel-ai-openapi.yml
  format: yaml
  label: Refuel Tasks API
  slug: refuel-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/refuel-ai/refs/heads/main/openapi/refuel-ai-openapi.yml
- filename: refuel-ai-openapi.yml
  format: yaml
  label: Refuel Datasets API
  slug: refuel-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/refuel-ai/refs/heads/main/openapi/refuel-ai-openapi.yml
- filename: refuel-ai-openapi.yml
  format: yaml
  label: Refuel Labeling and Predict API
  slug: refuel-labeling-predict-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/refuel-ai/refs/heads/main/openapi/refuel-ai-openapi.yml
- filename: refuel-ai-openapi.yml
  format: yaml
  label: Refuel Models API
  slug: refuel-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/refuel-ai/refs/heads/main/openapi/refuel-ai-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: refuel.ai
  spf: true
hosts:
- cert_expires: Sep 13 13:26:57 2026 GMT
  host: www.refuel.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 08:29:16 2026 GMT
  host: docs.refuel.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 23:59:59 2026 GMT
  host: cloud-api.refuel.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Refuel Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Refuel, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Refuel
provider_slug: refuel-ai
slug: refuel-ai-domain-security
source_filename: refuel-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.refuel.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 13:26:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.refuel.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 08:29:16 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: cloud-api.refuel.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: refuel.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/refuel-ai/refs/heads/main/security/refuel-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- LLM
- Data Labeling
- Data Enrichment
- Autolabel
---
