---
api_specs:
- filename: hilos-openapi-original.yml
  format: yaml
  label: Hilos API
  slug: hilos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hilos/refs/heads/main/openapi/hilos-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: hilos.io
  spf: false
hosts:
- cert_expires: Oct  8 06:08:48 2026 GMT
  host: hilos.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 06:08:48 2026 GMT
  host: api.hilos.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hilos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hilos, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Hilos
provider_slug: hilos
slug: hilos-domain-security
source_filename: hilos-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hilos.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 06:08:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.hilos.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 06:08:48 2026 GMT\n  hsts: null\ndomains:\n- domain: hilos.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hilos/refs/heads/main/security/hilos-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- WhatsApp
- Messaging
- Automation
- CRM
- Conversational Commerce
- Chatbots
- Customer Engagement
- Marketing
---
