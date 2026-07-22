---
api_specs:
- filename: structify-openapi-original.json
  format: json
  label: Structify API
  slug: structify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/structify/refs/heads/main/openapi/structify-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: structify.ai
  spf: true
hosts:
- cert_expires: Sep 22 10:48:38 2026 GMT
  host: structify.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 14 04:45:09 2026 GMT
  host: api.structify.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Structify Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Structify, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Structify
provider_slug: structify
slug: structify-domain-security
source_filename: structify-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: structify.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 10:48:38 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.structify.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 04:45:09 2026 GMT\n  hsts: null\ndomains:\n- domain: structify.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/structify/refs/heads/main/security/structify-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- Data
- Web Scraping
- Data Extraction
- Knowledge Graph
- ETL
- Data Enrichment
---
