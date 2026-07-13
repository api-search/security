---
api_specs:
- filename: sorsa-openapi.yml
  format: yaml
  label: Sorsa API v3
  slug: sorsa-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sorsa/refs/heads/main/openapi/sorsa-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: sorsa.io
  spf: true
hosts:
- cert_expires: Sep 16 04:51:34 2026 GMT
  host: sorsa.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 04:51:34 2026 GMT
  host: docs.sorsa.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 06:25:00 2026 GMT
  host: api.sorsa.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sorsa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sorsa, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Sorsa
provider_slug: sorsa
slug: sorsa-domain-security
source_filename: sorsa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sorsa.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 04:51:34 2026 GMT\n  hsts: false\n- host: docs.sorsa.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 04:51:34 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.sorsa.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 06:25:00 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: sorsa.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sorsa/refs/heads/main/security/sorsa-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Twitter
- X
- Social Media
- Data Extraction
- Real-Time
---
