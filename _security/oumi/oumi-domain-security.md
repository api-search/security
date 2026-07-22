---
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: oumi.ai
  spf: true
hosts:
- cert_expires: Jan  8 23:59:59 2027 GMT
  host: oumi.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 10 23:59:59 2027 GMT
  host: platform.oumi.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Oumi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Oumi, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Oumi
provider_slug: oumi
slug: oumi-domain-security
source_filename: oumi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: oumi.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 23:59:59 2027 GMT\n  hsts: false\n- host: platform.oumi.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 10 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: oumi.ai\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oumi/refs/heads/main/security/oumi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Economic Health
- Artificial Intelligence
- Machine Learning
- LLM
- Foundation Models
- Fine-Tuning
- Model Training
- Open Source
- MLOps
- Developer Tools
- Inference
---
