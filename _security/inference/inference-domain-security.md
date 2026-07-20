---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: inference.net
  spf: true
hosts:
- cert_expires: Oct  8 00:57:59 2026 GMT
  host: inference.net
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 02:54:15 2026 GMT
  host: docs.inference.net
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 00:16:17 2026 GMT
  host: api.inference.net
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Inference Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Inference, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Inference
provider_slug: inference
slug: inference-domain-security
source_filename: inference-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: inference.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 00:57:59 2026 GMT\n  hsts: false\n- host: docs.inference.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 02:54:15 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.inference.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 00:16:17 2026 GMT\n  hsts: null\ndomains:\n- domain: inference.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/inference/refs/heads/main/security/inference-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Machine Learning
- LLM
- Inference
- Observability
- Model Training
- Model Deployment
- MCP
- Crypto Web3
---
