---
api_specs:
- filename: autopass-openapi.yml
  format: yaml
  label: Autopass Service Authorization API
  slug: autopass-service-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autopass/refs/heads/main/openapi/autopass-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: autopass.xyz
  spf: true
hosts:
- cert_expires: Oct 15 02:01:11 2026 GMT
  host: en.autopass.xyz
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 23:26:55 2026 GMT
  host: docs.autopass.xyz
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  7 23:59:59 2026 GMT
  host: api.autopass.xyz
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Autopass Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Autopass, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Autopass
provider_slug: autopass
slug: autopass-domain-security
source_filename: autopass-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: en.autopass.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 02:01:11 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.autopass.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 23:26:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.autopass.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: autopass.xyz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/autopass/refs/heads/main/security/autopass-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Mobility
- Parking
- Payments
- Automotive
- Financial Services
- OAuth
- Taiwan
---
