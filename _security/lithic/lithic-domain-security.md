---
api_specs:
- filename: lithic-openapi.yml
  format: yaml
  label: Lithic REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lithic/refs/heads/main/openapi/lithic-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "sectigo.com"
  - 0 issue "amazonaws.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lithic.com
  spf: true
hosts:
- cert_expires: Oct  2 12:15:47 2026 GMT
  host: lithic.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 14:22:06 2026 GMT
  host: docs.lithic.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 23:59:59 2026 GMT
  host: api.lithic.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lithic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lithic, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Lithic
provider_slug: lithic
slug: lithic-domain-security
source_filename: lithic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lithic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 12:15:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.lithic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 14:22:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.lithic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: lithic.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lithic/refs/heads/main/security/lithic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- FinTech
- BaaS
- Card Issuing
- Payments
- Embedded Finance
---
