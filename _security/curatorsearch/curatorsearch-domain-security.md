---
api_specs:
- filename: curatorsearch-openapi.json
  format: json
  label: CuratorSearch API
  slug: curatorsearch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/curatorsearch/refs/heads/main/openapi/curatorsearch-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: curatorsearch.com
  spf: true
hosts:
- cert_expires: Nov 11 14:11:22 2026 GMT
  host: curatorsearch.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Curatorsearch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CuratorSearch, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: CuratorSearch
provider_slug: curatorsearch
slug: curatorsearch-domain-security
source_filename: curatorsearch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: curatorsearch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 14:11:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: curatorsearch.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/curatorsearch/refs/heads/main/security/curatorsearch-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Agent-Native
- MCP
- OpenAPI
- llms-txt
- Open Data
- Job
- Cultural Heritage
- Museums
- curatorial
- salary-transparency
- glam
- museum jobs
- Job Board
- Salaries
- Pay Transparency
- Datasets
- RSS
---
