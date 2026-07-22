---
api_specs:
- filename: select-star-openapi.yml
  format: yaml
  label: Select Star Metadata API
  slug: select-star-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/select-star/refs/heads/main/openapi/select-star-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: selectstar.com
  spf: true
hosts:
- cert_expires: Sep  2 18:22:59 2026 GMT
  host: docs.selectstar.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 25 23:59:59 2026 GMT
  host: api.production.selectstar.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Select Star Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Select Star, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Select Star
provider_slug: select-star
slug: select-star-domain-security
source_filename: select-star-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.selectstar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 18:22:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.production.selectstar.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: selectstar.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/select-star/refs/heads/main/security/select-star-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Data Catalog
- Data Lineage
- Metadata
- Data Governance
- Semantic Layer
- MCP
- AI-Ready Data
- Analytics
---
