---
api_specs:
- filename: pioneer-openapi-original.json
  format: json
  label: Pioneer Inference API
  slug: pioneer-inference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastino-labs/refs/heads/main/openapi/pioneer-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: fastino.ai
  spf: true
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  dmarc: false
  dnssec: false
  domain: pioneer.ai
  spf: true
hosts:
- cert_expires: Sep 26 03:35:02 2026 GMT
  host: www.fastino.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 12 23:59:59 2027 GMT
  host: api.pioneer.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fastino Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fastino Labs, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Fastino Labs
provider_slug: fastino-labs
slug: fastino-labs-domain-security
source_filename: fastino-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fastino.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 03:35:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.pioneer.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 12 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: fastino.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: pioneer.ai\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fastino-labs/refs/heads/main/security/fastino-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Small Language Models
- Fine-Tuning
- Inference
- Named Entity Recognition
- Information Extraction
- LLM
- Agents
- PII Detection
- Model Training
---
