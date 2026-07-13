---
api_specs:
- filename: rely-openapi.yml
  format: yaml
  label: Rely.io Public API
  slug: public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rely/refs/heads/main/openapi/rely-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "amazonaws.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: rely.io
  spf: true
hosts:
- host: www.rely.io
  https: false
- cert_expires: Sep 20 14:56:03 2026 GMT
  host: docs.rely.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.rely.io
  https: false
kind: domain-security
layout: security
method: probed
name: Rely Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rely.io, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Rely.io
provider_slug: rely
slug: rely-domain-security
source_filename: rely-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rely.io\n  https: false\n- host: docs.rely.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 14:56:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.rely.io\n  https: false\ndomains:\n- domain: rely.io\n  dnssec: true\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rely/refs/heads/main/security/rely-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Developer Experience
- Internal Developer Portal
- Platform Engineering
- Software Catalog
- Service Catalog
- Engineering Scorecards
---
