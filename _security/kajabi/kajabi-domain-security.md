---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Kajabi Public API
  slug: kajabi-public-api
  spec_type: OpenAPI
  url: https://github.com/Kajabi/public_api_docs/blob/main/openapi.yaml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: kajabi.com
  spf: true
hosts:
- cert_expires: Oct  4 09:05:49 2026 GMT
  host: www.kajabi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 18 23:44:13 2026 GMT
  host: help.kajabi.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 22 20:17:04 2026 GMT
  host: api.kajabi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kajabi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kajabi, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Kajabi
provider_slug: kajabi
slug: kajabi-domain-security
source_filename: kajabi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kajabi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 09:05:49 2026 GMT\n  hsts: false\n- host: help.kajabi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 23:44:13 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.kajabi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 20:17:04 2026 GMT\n  hsts: null\ndomains:\n- domain: kajabi.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kajabi/refs/heads/main/security/kajabi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Creator Economy
- Online Courses
- Memberships
- E-Commerce
- Digital Products
- Contacts
- Webhooks
- Payments
---
