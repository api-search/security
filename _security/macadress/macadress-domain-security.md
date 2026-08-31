---
api_specs:
- filename: macadress-openapi.yaml
  format: yaml
  label: macadress.com API
  slug: macadresscom-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/macadress/refs/heads/main/openapi/macadress-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: macadress.com
  spf: false
hosts:
- cert_expires: Oct 24 17:41:25 2026 GMT
  host: macadress.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 24 17:41:25 2026 GMT
  host: api.macadress.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Macadress Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MAC Address Lookup: Find Vendor, OUI & Device Type, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: 'MAC Address Lookup: Find Vendor, OUI & Device Type'
provider_slug: macadress
slug: macadress-domain-security
source_filename: macadress-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: macadress.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 17:41:25 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.macadress.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 17:41:25 2026 GMT\n  hsts: null\ndomains:\n- domain: macadress.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/macadress/refs/heads/main/security/macadress-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Networking
- Network Access Control
- Security
- SecOps
- IoT
- Device Fleet Management
- MDM
- Reference Data
- IEEE OUI Lookup
- Developer Tools
- MCP
- agent-native
---
