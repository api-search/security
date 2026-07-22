---
api_specs:
- filename: uselemma-platform-api-openapi-original.json
  format: json
  label: Lemma Platform API
  slug: uselemma-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uselemma/refs/heads/main/openapi/uselemma-platform-api-openapi-original.json
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: uselemma.ai
  spf: false
hosts:
- cert_expires: Oct  6 22:09:29 2026 GMT
  host: www.uselemma.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 22:09:29 2026 GMT
  host: docs.uselemma.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 22:09:29 2026 GMT
  host: api.uselemma.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Uselemma Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lemma, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=none).'
provider_name: Lemma
provider_slug: uselemma
slug: uselemma-domain-security
source_filename: uselemma-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.uselemma.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 22:09:29 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.uselemma.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 22:09:29 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.uselemma.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 22:09:29 2026 GMT\n  hsts: false\ndomains:\n- domain: uselemma.ai\n  dnssec: true\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uselemma/refs/heads/main/security/uselemma-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Artificial Intelligence
- AI Agents
- Observability
- Monitoring
- Tracing
- Developer Tools
- B2B
---
