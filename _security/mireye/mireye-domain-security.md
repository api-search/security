---
api_specs:
- filename: mireye-openapi-original.json
  format: json
  label: Mireye Earth API
  slug: mireye-earth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mireye/refs/heads/main/openapi/mireye-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mireye.ai
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mireye.com
  spf: true
hosts:
- cert_expires: Aug 23 09:37:06 2026 GMT
  host: docs.mireye.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 05:35:34 2026 GMT
  host: api.mireye.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mireye Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mireye, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Mireye
provider_slug: mireye
slug: mireye-domain-security
source_filename: mireye-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.mireye.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 09:37:06 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.mireye.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 05:35:34 2026 GMT\n  hsts: null\ndomains:\n- domain: mireye.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: mireye.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mireye/refs/heads/main/security/mireye-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Geospatial
- Geographic Information System
- Location
- AI Agents
- Model Context Protocol
- Government Data
- Risk
- Insurance
- Data
---
