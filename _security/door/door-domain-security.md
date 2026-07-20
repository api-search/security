---
api_specs:
- filename: door-partner-openapi.json
  format: json
  label: OpenDOOR Partner API
  slug: opendoor-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/door/refs/heads/main/openapi/door-partner-openapi.json
- filename: door-authentication-openapi.json
  format: json
  label: OpenDOOR Authentication API
  slug: opendoor-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/door/refs/heads/main/openapi/door-authentication-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: door.com
  spf: true
hosts:
- cert_expires: Aug 23 16:48:14 2026 GMT
  host: door.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Door Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Door, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Door
provider_slug: door
slug: door-domain-security
source_filename: door-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: door.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 16:48:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: door.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/door/refs/heads/main/security/door-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Access Control
- Smart Building
- Proptech
- Physical Security
- IoT
- Multifamily
- Real Estate
- Smart Lock
- Building Automation
---
