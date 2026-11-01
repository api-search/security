---
api_specs:
- filename: siftwright-com-api-openapi.json
  format: json
  label: Siftwright API API
  slug: siftwright-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/siftwright-com/openapi/_original/siftwright-com-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: siftwright.com
  spf: true
hosts:
- cert_expires: Dec 27 15:11:17 2026 GMT
  host: siftwright.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Siftwright Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for siftwright-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: siftwright-com
provider_slug: siftwright-com
slug: siftwright-com-domain-security
source_filename: siftwright-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: siftwright.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 15:11:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: siftwright.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/siftwright-com/security/siftwright-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- API
- Data
- AI
- Web-Data
---
