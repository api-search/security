---
api_specs:
- filename: tesslio-openapi-original.json
  format: json
  label: Tessl API
  slug: tessl-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tesslio/refs/heads/main/openapi/tesslio-openapi-original.json
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:security@tessl.io"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tessl.io
  spf: true
hosts:
- cert_expires: Sep 21 13:30:30 2026 GMT
  host: tessl.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 13:30:33 2026 GMT
  host: api.tessl.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tesslio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for tessl.io, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: tessl.io
provider_slug: tesslio
slug: tesslio-domain-security
source_filename: tesslio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tessl.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 13:30:30 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.tessl.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 13:30:33 2026 GMT\n  hsts: null\ndomains:\n- domain: tessl.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:security@tessl.io\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tesslio/refs/heads/main/security/tesslio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai Ml
- Agent Enablement
- Agentic Development
- Developer Tools
- Skills Registry
- Model Context Protocol
- Spec-Driven Development
- Code Review
- CLI
---
