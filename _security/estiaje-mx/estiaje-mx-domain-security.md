---
api_specs:
- filename: estiaje-mx-openapi-generated.yml
  format: yaml
  label: Estiaje API
  slug: estiaje-mx-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/estiaje-mx/openapi/_ae-authored/estiaje-mx-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: estiaje.mx
  spf: true
hosts:
- cert_expires: Jan 31 10:37:25 2027 GMT
  host: estiaje.mx
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Estiaje Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Estiaje, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Estiaje
provider_slug: estiaje-mx
slug: estiaje-mx-domain-security
source_filename: estiaje-mx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: estiaje.mx\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 10:37:25 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: estiaje.mx\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/estiaje-mx/security/estiaje-mx-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Payments
- Alerts
- Mexico
---
