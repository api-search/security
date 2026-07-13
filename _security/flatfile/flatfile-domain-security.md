---
api_specs:
- filename: flatfile-api-openapi.yml
  format: yaml
  label: Flatfile API
  slug: flatfile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flatfile/refs/heads/main/openapi/flatfile-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: flatfile.com
  spf: true
hosts:
- cert_expires: Sep  7 14:14:08 2026 GMT
  host: flatfile.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 15:09:28 2026 GMT
  host: reference.flatfile.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 11:21:11 2026 GMT
  host: api.x.flatfile.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Flatfile Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flatfile, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Flatfile
provider_slug: flatfile
slug: flatfile-domain-security
source_filename: flatfile-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: flatfile.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 14:14:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: reference.flatfile.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 15:09:28 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.x.flatfile.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 11:21:11 2026 GMT\n  hsts: null\ndomains:\n- domain: flatfile.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flatfile/refs/heads/main/security/flatfile-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Data Exchange
- Data Ingestion
- Data Onboarding
- Data Validation
- ETL
- File Import
---
