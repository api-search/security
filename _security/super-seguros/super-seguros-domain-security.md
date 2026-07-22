---
api_specs:
- filename: super-seguros-openapi.json
  format: json
  label: Super Studio API
  slug: super-studio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/super-seguros/refs/heads/main/openapi/super-seguros-openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: super.mx
  spf: true
hosts:
- cert_expires: Feb  4 23:59:59 2027 GMT
  host: www.super.mx
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 16:31:31 2026 GMT
  host: developers.super.mx
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 25 16:38:44 2026 GMT
  host: app.super.mx
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Super Seguros Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Super Seguros, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Super Seguros
provider_slug: super-seguros
slug: super-seguros-domain-security
source_filename: super-seguros-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.super.mx\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 23:59:59 2027 GMT\n  hsts: false\n- host: developers.super.mx\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 16:31:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.super.mx\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 16:38:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: super.mx\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/super-seguros/refs/heads/main/security/super-seguros-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Insurance
- Insurtech
- Life Insurance
- Quotes
- Mexico
- Financial Services
- Super Studio
---
