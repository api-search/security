---
api_specs:
- filename: hpt-su-openapi-generated.yml
  format: yaml
  label: HPT.SU API
  slug: hpt-su-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hpt-su/openapi/_ae-authored/hpt-su-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hpt.su
  spf: true
hosts:
- cert_expires: Dec 21 17:27:46 2026 GMT
  host: hpt.su
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: HPT.SU Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HPT.SU, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: HPT.SU
provider_slug: hpt-su
slug: hpt-su-domain-security
source_filename: hpt-su-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hpt.su\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 17:27:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hpt.su\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/hpt-su/security/hpt-su-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Vehicles
- Documentation
- Russian
- Automotive
---
