---
api_specs:
- filename: sambanova-systems-cloud-openapi-original.yml
  format: yaml
  label: SambaNova Cloud API
  slug: sambanova-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sambanova-systems/refs/heads/main/openapi/sambanova-systems-cloud-openapi-original.yml
- filename: sambanova-systems-agents-openapi-original.yml
  format: yaml
  label: SambaNova Agents Service
  slug: sambanova-agents-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sambanova-systems/refs/heads/main/openapi/sambanova-systems-agents-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sambanovasystems.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: sambanova.ai
  spf: true
hosts:
- cert_expires: Oct 17 21:40:44 2026 GMT
  host: sambanovasystems.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 31 22:47:18 2026 GMT
  host: chat.sambanova.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 17 23:04:00 2027 GMT
  host: api.sambanova.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sambanova Systems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SambaNova Systems, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: SambaNova Systems
provider_slug: sambanova-systems
slug: sambanova-systems-domain-security
source_filename: sambanova-systems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sambanovasystems.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 21:40:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: chat.sambanova.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 31 22:47:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.sambanova.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 23:04:00 2027 GMT\n  hsts: null\ndomains:\n- domain: sambanovasystems.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: sambanova.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sambanova-systems/refs/heads/main/security/sambanova-systems-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Ai
- Artificial Intelligence
- Machine Learning
- LLM
- Inference
- Generative AI
- API
- Agents
- Embeddings
---
