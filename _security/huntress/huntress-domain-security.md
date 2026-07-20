---
api_specs:
- filename: huntress-rest-openapi.json
  format: json
  label: Huntress REST API
  slug: huntress-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/huntress/refs/heads/main/openapi/huntress-rest-openapi.json
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: huntress.com
  spf: true
- caa:
  - 0 issuewild "digicert.com"
  - 0 iodef "mailto:security@huntress.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: huntress.io
  spf: true
hosts:
- cert_expires: Jan 27 23:59:59 2027 GMT
  host: www.huntress.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan 28 23:59:59 2027 GMT
  host: api.huntress.io
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Huntress Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Huntress, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Huntress
provider_slug: huntress
slug: huntress-domain-security
source_filename: huntress-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.huntress.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 27 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.huntress.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 28 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: huntress.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: huntress.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com\"\n  - 0 iodef \"mailto:security@huntress.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/huntress/refs/heads/main/security/huntress-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Security
- Cybersecurity
- Managed Detection and Response
- Endpoint Security
- SOC
- SIEM
- Identity Threat Detection
- MSP
- Webhooks
---
