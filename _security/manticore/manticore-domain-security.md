---
api_specs:
- filename: manticore.yml
  format: yaml
  label: Manticore Search REST API
  slug: manticore-search-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/manticoresoftware/openapi/master/manticore.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: manticoresearch.com
  spf: true
hosts:
- cert_expires: Oct  7 23:19:00 2026 GMT
  host: manticoresearch.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 13:56:59 2026 GMT
  host: manual.manticoresearch.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: 127.0.0.1
  https: false
kind: domain-security
layout: security
method: probed
name: Manticore Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Manticore Search, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Manticore Search
provider_slug: manticore
slug: manticore-domain-security
source_filename: manticore-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: manticoresearch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 23:19:00 2026 GMT\n  hsts: false\n- host: manual.manticoresearch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 13:56:59 2026 GMT\n  hsts: false\n- host: 127.0.0.1\n  https: false\ndomains:\n- domain: manticoresearch.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/manticore/refs/heads/main/security/manticore-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Search
- Full-Text Search
- Vector Search
- Elasticsearch Compatible
- Open Source
- Database
---
