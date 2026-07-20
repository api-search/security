---
api_specs:
- filename: howler-consumer-portal-openapi.yml
  format: yaml
  label: Howler API v3 (Consumer Portal)
  slug: howler-api-v3-consumer-portal
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/howler/refs/heads/main/openapi/howler-consumer-portal-openapi.yml
- filename: howler-webhooks-openapi.yml
  format: yaml
  label: Howler Webhooks v1
  slug: howler-webhooks-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/howler/refs/heads/main/openapi/howler-webhooks-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: howler.co.za
  spf: true
hosts:
- cert_expires: Jan 13 23:59:59 2027 GMT
  host: howler.co.za
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Howler Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Howler, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Howler
provider_slug: howler
slug: howler-domain-security
source_filename: howler-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: howler.co.za\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: howler.co.za\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/howler/refs/heads/main/security/howler-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Events
- Ticketing
- Payments
- Cashless
- RFID
- Event Management
- Fintech
- South Africa
---
