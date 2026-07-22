---
api_specs:
- filename: understudy-labs-desktop-api-openapi.json
  format: json
  label: Understudy Desktop Agent API
  slug: understudy-desktop-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/understudy-labs/refs/heads/main/openapi/understudy-labs-desktop-api-openapi.json
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: understudylabs.com
  spf: true
hosts:
- cert_expires: Sep 25 01:42:25 2026 GMT
  host: understudylabs.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 23 23:29:44 2026 GMT
  host: docs.understudylabs.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 00:54:29 2026 GMT
  host: api.understudylabs.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Understudy Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Understudy Labs, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Understudy Labs
provider_slug: understudy-labs
slug: understudy-labs-domain-security
source_filename: understudy-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: understudylabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 01:42:25 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.understudylabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 23 23:29:44 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.understudylabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 00:54:29 2026 GMT\n  hsts: false\ndomains:\n- domain: understudylabs.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/understudy-labs/refs/heads/main/security/understudy-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- LLM Gateway
- Machine Learning
- Open Source
- Model Routing
- Evaluations
- Fine-Tuning
- AI Infrastructure
- Developer Tools
---
