---
api_specs:
- filename: handy-orders-openapi.json
  format: json
  label: Handy Partner Orders API
  slug: handy-partner-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/handy/refs/heads/main/openapi/handy-orders-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: handy.com
  spf: true
hosts:
- cert_expires: Dec 31 23:59:59 2026 GMT
  host: handy.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Handy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for handy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: handy
provider_slug: handy
slug: handy-domain-security
source_filename: handy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: handy.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 31 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: handy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/handy/refs/heads/main/security/handy-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Home Services
- Marketplace
- Cleaning
- Handyman
- Installations
- On-Demand
- Gig Economy
- Orders
- Webhooks
- Retail
- Angi
---
