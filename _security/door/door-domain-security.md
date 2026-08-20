---
api_specs:
- filename: door-access-management-api-openapi.yml
  format: yaml
  label: Door Access Management API
  slug: door-access-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/door/refs/heads/main/openapi/door-access-management-api-openapi.yml
- filename: door-buildings-api-openapi.yml
  format: yaml
  label: Door Buildings API
  slug: door-buildings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/door/refs/heads/main/openapi/door-buildings-api-openapi.yml
- filename: door-doors-and-keys-api-openapi.yml
  format: yaml
  label: Door Doors and Keys API
  slug: door-doors-and-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/door/refs/heads/main/openapi/door-doors-and-keys-api-openapi.yml
- filename: door-partner-authentication-api-openapi.yml
  format: yaml
  label: Door Partner Authentication API
  slug: door-partner-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/door/refs/heads/main/openapi/door-partner-authentication-api-openapi.yml
- filename: door-user-authentication-api-openapi.yml
  format: yaml
  label: Door User Authentication API
  slug: door-user-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/door/refs/heads/main/openapi/door-user-authentication-api-openapi.yml
- filename: door-users-api-openapi.yml
  format: yaml
  label: Door Users API
  slug: door-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/door/refs/heads/main/openapi/door-users-api-openapi.yml
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
- PropTech
- Physical Security
- IoT
- Multifamily
- Real-Estate
- Smart Lock
- Building Automation
---
