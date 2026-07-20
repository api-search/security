---
api_specs:
- filename: openapi.json
  format: json
  label: Alloovium API
  slug: alloovium-api
  spec_type: OpenAPI
  url: https://api.alloovium.com/api/v2/openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: alloovium.com
  spf: true
hosts:
- cert_expires: Oct 14 06:20:09 2026 GMT
  host: www.alloovium.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.alloovium.com
  https: false
kind: domain-security
layout: security
method: probed
name: Alloovium Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alloovium, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Alloovium
provider_slug: alloovium
slug: alloovium-domain-security
source_filename: alloovium-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.alloovium.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 06:20:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.alloovium.com\n  https: false\ndomains:\n- domain: alloovium.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alloovium/refs/heads/main/security/alloovium-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Construction
- Document Intelligence
- Compliance
- Artificial Intelligence
- Construction Technology
- Documents
- MCP
---
