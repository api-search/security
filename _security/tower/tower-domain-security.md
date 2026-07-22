---
api_specs:
- filename: tower-openapi-original.json
  format: json
  label: Tower API
  slug: tower-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tower/refs/heads/main/openapi/tower-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tower.dev
  spf: true
hosts:
- cert_expires: Jan 19 23:59:59 2027 GMT
  host: tower.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 11 23:59:59 2026 GMT
  host: docs.tower.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 11 23:59:59 2026 GMT
  host: api.tower.dev
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Tower Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tower, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Tower
provider_slug: tower
slug: tower-domain-security
source_filename: tower-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tower.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 23:59:59 2027 GMT\n  hsts: false\n- host: docs.tower.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 23:59:59 2026 GMT\n  hsts: false\n- host: api.tower.dev\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 11 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: tower.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tower/refs/heads/main/security/tower-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Data Infrastructure
- Data Engineering
- Python
- Apache Iceberg
- Lakehouse
- Orchestration
- Data Pipelines
- AI Agents
- MCP
- ETL
---
