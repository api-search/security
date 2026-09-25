---
api_specs:
- filename: ingest0r-com-openapi.yml
  format: yaml
  label: Cook County (Chicago) Property Records API
  slug: cook-county-property-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ingest0r-com/refs/heads/main/openapi/ingest0r-com-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ingest0r.com
  spf: false
hosts:
- cert_expires: Nov  8 15:58:20 2026 GMT
  host: api.ingest0r.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ingest0R Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ingest0r, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: ingest0r
provider_slug: ingest0r-com
slug: ingest0r-com-domain-security
source_filename: ingest0r-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.ingest0r.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 15:58:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ingest0r.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ingest0r-com/refs/heads/main/security/ingest0r-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Real Estate
- Property Records
- Property Data
- Public Records
- Open Data
- Government Data
- Parcel
- Geocoding
- Property Tax
- Building Permits
- Comparable Sales
- Valuation
- x402
- Agentic Commerce
- MCP
- A2A
- Agent-Native
- Chicago
- Illinois
---
