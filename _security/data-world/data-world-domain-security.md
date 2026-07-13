---
api_specs:
- filename: openapi.json
  format: json
  label: data.world REST API
  slug: dataworld-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/data-world/refs/heads/main/openapi/openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: data.world
  spf: true
hosts:
- cert_expires: Aug 26 21:28:09 2026 GMT
  host: developer.data.world
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 03:33:08 2026 GMT
  host: api.data.world
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Data World Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for data.world, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: data.world
provider_slug: data-world
slug: data-world-domain-security
source_filename: data-world-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.data.world\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 21:28:09 2026 GMT\n  hsts: null\n- host: api.data.world\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 13 03:33:08 2026 GMT\n  hsts: null\ndomains:\n- domain: data.world\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/data-world/refs/heads/main/security/data-world-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Data Catalog
- Data Governance
- Metadata Management
- SPARQL
- SQL
- Open Data
- Collaboration
---
