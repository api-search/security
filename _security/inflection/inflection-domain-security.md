---
api_specs:
- filename: inflection-chat-api-openapi.yml
  format: yaml
  label: Inflection AI Chat API
  slug: inflection-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inflection/refs/heads/main/openapi/inflection-chat-api-openapi.yml
- filename: inflection-discovery-api-openapi.yml
  format: yaml
  label: Inflection AI Discovery API
  slug: inflection-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inflection/refs/heads/main/openapi/inflection-discovery-api-openapi.yml
- filename: inflection-embeddings-api-openapi.yml
  format: yaml
  label: Inflection AI Embeddings API
  slug: inflection-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inflection/refs/heads/main/openapi/inflection-embeddings-api-openapi.yml
- filename: inflection-external-api-openapi.yml
  format: yaml
  label: Inflection AI External API
  slug: inflection-external-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inflection/refs/heads/main/openapi/inflection-external-api-openapi.yml
- filename: inflection-status-api-openapi.yml
  format: yaml
  label: Inflection AI Status API
  slug: inflection-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inflection/refs/heads/main/openapi/inflection-status-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: inflection.ai
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: inf7ks8.com
  spf: false
hosts:
- cert_expires: Oct  7 15:01:53 2026 GMT
  host: inflection.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 21 21:22:43 2026 GMT
  host: developers.inflection.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 06:03:32 2026 GMT
  host: layercake.pubwestus3.inf7ks8.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Inflection Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Inflection AI, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Inflection AI
provider_slug: inflection
slug: inflection-domain-security
source_filename: inflection-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: inflection.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 15:01:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.inflection.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 21:22:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: layercake.pubwestus3.inf7ks8.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 06:03:32 2026 GMT\n  hsts: null\ndomains:\n- domain: inflection.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: inf7ks8.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/inflection/refs/heads/main/security/inflection-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- LLM
- Personal AI
- Pi
- Foundation Models
- Empathetic AI
---
