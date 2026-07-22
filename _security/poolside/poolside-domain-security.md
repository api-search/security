---
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: poolside.ai
  spf: true
hosts:
- cert_expires: Oct  4 14:53:52 2026 GMT
  host: docs.poolside.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 01:16:15 2026 GMT
  host: inference.poolside.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Poolside Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for poolside, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: poolside
provider_slug: poolside
slug: poolside-domain-security
source_filename: poolside-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.poolside.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 14:53:52 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: inference.poolside.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 01:16:15 2026 GMT\n  hsts: null\ndomains:\n- domain: poolside.ai\n  dnssec: false\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/poolside/refs/heads/main/security/poolside-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Enterprise
- Artificial Intelligence
- Machine Learning
- Foundation Models
- Coding Assistant
- Developer Tools
- LLM
- Agents
- Code Generation
- Inference
- OpenAI Compatible
---
