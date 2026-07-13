---
api_specs:
- filename: parcellab-openapi.yml
  format: yaml
  label: parcelLab API
  slug: parcellab-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parcellab/refs/heads/main/openapi/parcellab-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "sectigo.com"
  - 0 issuewild "ssl.com"
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: parcellab.com
  spf: true
hosts:
- cert_expires: Sep  8 17:46:26 2026 GMT
  host: parcellab.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 15:32:50 2026 GMT
  host: docs.parcellab.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 23:59:59 2026 GMT
  host: api.parcellab.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Parcellab Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for parcelLab, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: parcelLab
provider_slug: parcellab
slug: parcellab-domain-security
source_filename: parcellab-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: parcellab.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 17:46:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.parcellab.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 15:32:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.parcellab.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: parcellab.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/parcellab/refs/heads/main/security/parcellab-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Post-Purchase
- E-Commerce
- Tracking
- Returns
- Shipping
- Delivery
- Customer Experience
- Logistics
- Communications
- Germany
---
