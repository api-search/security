---
api_specs:
- filename: ready2order-openapi-original.json
  format: json
  label: ready2order Public API
  slug: ready2order-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ready2order/refs/heads/main/openapi/ready2order-openapi-original.json
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ready2order.com
  spf: true
hosts:
- cert_expires: Oct 14 23:59:59 2026 GMT
  host: api.ready2order.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Ready2Order Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ready2order, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ready2order
provider_slug: ready2order
slug: ready2order-domain-security
source_filename: ready2order-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.ready2order.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 14 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ready2order.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ready2order/refs/heads/main/security/ready2order-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Point of Sale
- POS
- Payments
- Retail
- Gastronomy
- Cash Register
- SaaS
---
