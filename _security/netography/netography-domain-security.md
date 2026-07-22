---
api_specs:
- filename: netography-openapi.yml
  format: yaml
  label: Netography (Vectra Fusion) API
  slug: netography-vectra-fusion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netography/refs/heads/main/openapi/netography-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: netography.com
  spf: true
hosts:
- cert_expires: Dec 30 23:59:59 2026 GMT
  host: netography.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Netography Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Netography, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Netography
provider_slug: netography
slug: netography-domain-security
source_filename: netography-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: netography.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: netography.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/netography/refs/heads/main/security/netography-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Network Security
- Network Detection and Response
- Cloud Security
- Network Observability
- Flow Data
- Threat Intelligence
- DDoS
- Cybersecurity
- MITRE ATT&CK
- Company
---
