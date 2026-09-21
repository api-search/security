---
api_specs:
- filename: ozan-soft-openapi.yml
  format: yaml
  label: GenderAPI.io
  slug: genderapiio
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ozan-soft/refs/heads/main/openapi/ozan-soft-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: genderapi.io
  spf: true
hosts:
- cert_expires: Nov 14 10:54:55 2026 GMT
  host: www.genderapi.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 16 16:03:46 2026 GMT
  host: api.genderapi.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Ozan Soft Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ozan Soft, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Ozan Soft
provider_slug: ozan-soft
slug: ozan-soft-domain-security
source_filename: ozan-soft-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.genderapi.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 10:54:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.genderapi.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 16 16:03:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: genderapi.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ozan-soft/refs/heads/main/security/ozan-soft-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Data Enrichment
- Gender Detection
- Name Analysis
- Demographics
- Identity
- Marketing Data
- Developer API
- Phone Validation
---
