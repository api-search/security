---
api_specs:
- filename: squillo-platform-openapi.yml
  format: yaml
  label: Squillo Platform API
  slug: squillo-platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/squillo/refs/heads/main/openapi/squillo-platform-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild ";"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  dmarc: false
  dnssec: false
  domain: squillo.io
  spf: true
hosts:
- cert_expires: Oct  1 08:24:52 2026 GMT
  host: squillo.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- host: api.squillo.io
  https: false
kind: domain-security
layout: security
method: probed
name: Squillo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Squillo, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Squillo
provider_slug: squillo
slug: squillo-domain-security
source_filename: squillo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: squillo.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 08:24:52 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.squillo.io\n  https: false\ndomains:\n- domain: squillo.io\n  dnssec: false\n  caa:\n  - 0 issuewild \";\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/squillo/refs/heads/main/security/squillo-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Integration Platform
- Automation
- Workflow
- No-Code
- IT Process Automation
- Software As A Utility
---
