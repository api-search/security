---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 iodef "mailto:security+caa@wandb.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: wandb.ai
  spf: true
hosts:
- cert_expires: Sep  8 22:58:04 2026 GMT
  host: wandb.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 20:23:08 2026 GMT
  host: docs.wandb.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 15 19:57:25 2026 GMT
  host: api.wandb.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Weights And Biases Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Weights & Biases, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Weights & Biases
provider_slug: weights-and-biases
slug: weights-and-biases-domain-security
source_filename: weights-and-biases-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wandb.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 22:58:04 2026 GMT\n  hsts: false\n- host: docs.wandb.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 20:23:08 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.wandb.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 19:57:25 2026 GMT\n  hsts: null\ndomains:\n- domain: wandb.ai\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 iodef \"mailto:security+caa@wandb.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/weights-and-biases/refs/heads/main/security/weights-and-biases-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- ML
- MLOps
- Experiment Tracking
- Model Registry
- GenAI
---
