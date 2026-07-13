---
api_specs:
- filename: snipcart-rest-api-openapi.yml
  format: yaml
  label: Snipcart REST API
  slug: snipcart-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snipcart/refs/heads/main/openapi/snipcart-rest-api-openapi.yml
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
  domain: snipcart.com
  spf: true
hosts:
- cert_expires: Sep 10 09:23:56 2026 GMT
  host: snipcart.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 15 16:53:56 2026 GMT
  host: docs.snipcart.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  9 23:59:59 2026 GMT
  host: app.snipcart.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Snipcart Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Snipcart, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Snipcart
provider_slug: snipcart
slug: snipcart-domain-security
source_filename: snipcart-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: snipcart.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 09:23:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.snipcart.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 16:53:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.snipcart.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: snipcart.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/snipcart/refs/heads/main/security/snipcart-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- E-Commerce
- Shopping Cart
- Orders
- Products
- Payments
- Webhooks
- Headless Commerce
- Jamstack
---
