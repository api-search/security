---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: makeBIMI SVG Validation API
  slug: makebimi-validation-api
  spec_type: OpenAPI
  url: https://makebimi.com/public/openapi.yaml
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: makebimi.com
  spf: true
hosts:
- cert_expires: Nov 29 09:50:09 2026 GMT
  host: makebimi.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Makebimi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for makeBIMI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: makeBIMI
provider_slug: makebimi
slug: makebimi-domain-security
source_filename: makebimi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: makebimi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 09:50:09 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: makebimi.com\n  dnssec: true\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/makebimi/refs/heads/main/security/makebimi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- BIMI
- DMARC
- Email Authentication
- SVG
- brand indicators
- SVG validation
---
