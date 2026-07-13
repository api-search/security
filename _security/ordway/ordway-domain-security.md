---
api_specs:
- filename: ordway-rest-api-openapi.yml
  format: yaml
  label: Ordway REST API
  slug: ordway-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordway/refs/heads/main/openapi/ordway-rest-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ordwaylabs.com
  spf: true
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:devops@stoplight.io"
  - 0 issue "cloudflare.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: stoplight.io
  spf: true
hosts:
- cert_expires: Aug 21 12:29:03 2026 GMT
  host: ordwaylabs.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 22:17:08 2026 GMT
  host: ordwaylabs.stoplight.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  6 23:59:59 2027 GMT
  host: api.ordwaylabs.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ordway Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ordway, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ordway
provider_slug: ordway
slug: ordway-domain-security
source_filename: ordway-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ordwaylabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 12:29:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: ordwaylabs.stoplight.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 22:17:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.ordwaylabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: ordwaylabs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: stoplight.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:devops@stoplight.io\"\n  - 0 issue \"cloudflare.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ordway/refs/heads/main/security/ordway-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Billing
- Revenue Automation
- Subscriptions
- Invoicing
- Payments
- Revenue Recognition
- SaaS Metrics
- Usage-Based Billing
- Financial Reporting
- Accounts Receivable
---
