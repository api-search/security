---
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mistral.ai
  spf: true
hosts:
- cert_expires: Sep 11 21:38:58 2026 GMT
  host: mistral.ai
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 16:46:55 2026 GMT
  host: docs.mistral.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 21:30:01 2026 GMT
  host: api.mistral.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mistralai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mistral AI, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Mistral AI
provider_slug: mistralai
slug: mistralai-domain-security
source_filename: mistralai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mistral.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 21:38:58 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: docs.mistral.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 16:46:55 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.mistral.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 21:30:01 2026 GMT\n  hsts: null\ndomains:\n- domain: mistral.ai\n  dnssec: false\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mistralai/refs/heads/main/security/mistralai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Large Language Models
- Generative AI
- Machine Learning
- Chat
- Embeddings
- Agents
- OCR
- Fine-Tuning
- Developer Platform
---
