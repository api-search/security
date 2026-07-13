---
api_specs:
- filename: corporate-bullshit-generator-api-openapi.yml
  format: yaml
  label: Corporate Bullshit Generator API
  slug: cbsg-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/corporate-bullshit-generator-api/refs/heads/main/openapi/corporate-bullshit-generator-api-openapi.yml
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
  dmarc_policy: none
  dnssec: false
  domain: sameerkumar.website
  spf: true
hosts:
- cert_expires: Aug 29 17:18:13 2026 GMT
  host: corporatebs-generator.sameerkumar.website
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Corporate Bullshit Generator Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Corporate Bullshit Generator API, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Corporate Bullshit Generator API
provider_slug: corporate-bullshit-generator-api
slug: corporate-bullshit-generator-api-domain-security
source_filename: corporate-bullshit-generator-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: corporatebs-generator.sameerkumar.website\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 17:18:13 2026 GMT\n  hsts: false\ndomains:\n- domain: sameerkumar.website\n  dnssec: false\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/corporate-bullshit-generator-api/refs/heads/main/security/corporate-bullshit-generator-api-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Buzzwords
- Comedy
- Corporate Jargon
- Fake Data
- Free
- Generator
- JSON
- Mock Data
- Phrases
- Public API
- REST
- Test Data
- Unauthenticated
---
