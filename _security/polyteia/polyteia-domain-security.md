---
api_specs:
- filename: polyteia-platform-openapi.yml
  format: yaml
  label: Polyteia Platform API
  slug: polyteia-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polyteia/refs/heads/main/openapi/polyteia-platform-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "sectigo.com"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  dmarc: false
  dnssec: false
  domain: polyteia.com
  spf: true
hosts:
- cert_expires: Sep  7 22:56:02 2026 GMT
  host: app.polyteia.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Polyteia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Polyteia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Polyteia
provider_slug: polyteia
slug: polyteia-domain-security
source_filename: polyteia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: app.polyteia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 22:56:02 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: polyteia.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/polyteia/refs/heads/main/security/polyteia-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Ai Enterprise Software
- GovTech
- Public Sector
- Data Platform
- Government
- Data Analytics
- Germany
- Business Intelligence
- No-Code
---
