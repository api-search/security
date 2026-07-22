---
api_specs:
- filename: starbridge-openapi.json
  format: json
  label: Starbridge External Public API
  slug: starbridge-external-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/starbridge/refs/heads/main/openapi/starbridge-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: starbridge.ai
  spf: true
hosts:
- cert_expires: Sep  8 06:36:20 2026 GMT
  host: starbridge.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Starbridge Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Starbridge, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Starbridge
provider_slug: starbridge
slug: starbridge-domain-security
source_filename: starbridge-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: starbridge.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 06:36:20 2026 GMT\n  hsts: false\ndomains:\n- domain: starbridge.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/starbridge/refs/heads/main/security/starbridge-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Ai
- Sales Intelligence
- Go To Market
- Public Sector
- Education
- Government
- Procurement
- Buyer Intelligence
- MCP
---
