---
api_specs:
- filename: signzy-authentication-api-openapi.yml
  format: yaml
  label: Signzy Authentication API
  slug: signzy-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signzy/refs/heads/main/openapi/signzy-authentication-api-openapi.yml
- filename: signzy-banking-api-openapi.yml
  format: yaml
  label: Signzy Banking API
  slug: signzy-banking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signzy/refs/heads/main/openapi/signzy-banking-api-openapi.yml
- filename: signzy-identity-india-api-openapi.yml
  format: yaml
  label: Signzy Identity (India) API
  slug: signzy-identity-india-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signzy/refs/heads/main/openapi/signzy-identity-india-api-openapi.yml
- filename: signzy-identity-us-api-openapi.yml
  format: yaml
  label: Signzy Identity (US) API
  slug: signzy-identity-us-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signzy/refs/heads/main/openapi/signzy-identity-us-api-openapi.yml
description: ''
domains:
- data_localization: true
  domain: signzy.com
  encryption: 256-bit SSL/TLS
  notes: Signzy advertises 256-bit SSL encryption, data localization / residency, FATF compliance, and 24x7 security incident & event monitoring.
hosts:
- cert_expires: Aug 29 01:06:54 2026 GMT
  host: www.signzy.com
  hsts: true
  hsts_max_age: 63072000
  http_status: 200
  https: true
- host: docs.signzy.com
  hsts: null
  http_status: 200
  https: true
  note: Documentation portal fronted by Cloudflare.
- cert_expires: Nov 23 23:59:59 2026 GMT
  host: api.signzy.app
  hsts: null
  http_status: 401
  https: true
  note: Production API host; 401 at root confirms authenticated REST surface.
- host: api-preproduction.signzy.app
  hsts: null
  http_status: 404
  https: true
  note: Preproduction / sandbox API host; 404 at root (no index route).
kind: domain-security
layout: security
method: probed
name: Signzy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Signzy, probed live across 4 host(s) and 1 registrable domain(s). 4 host(s) serve HTTPS; 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Signzy
provider_slug: signzy
slug: signzy-domain-security
source_filename: signzy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.signzy.com\n  https: true\n  http_status: 200\n  cert_expires: Aug 29 01:06:54 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.signzy.com\n  https: true\n  http_status: 200\n  hsts: null\n  note: Documentation portal fronted by Cloudflare.\n- host: api.signzy.app\n  https: true\n  http_status: 401\n  cert_expires: Nov 23 23:59:59 2026 GMT\n  hsts: null\n  note: Production API host; 401 at root confirms authenticated REST surface.\n- host: api-preproduction.signzy.app\n  https: true\n  http_status: 404\n  hsts: null\n  note: Preproduction / sandbox API host; 404 at root (no index route).\ndomains:\n- domain: signzy.com\n  encryption: 256-bit SSL/TLS\n  data_localization: true\n  notes: >-\n    Signzy advertises 256-bit SSL encryption, data localization / residency,\n    FATF compliance, and 24x7 security incident & event monitoring.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/signzy/refs/heads/main/security/signzy-domain-security.yml
summary_line: HSTS
tags:
- Identity Verification
- KYC
- KYB
- AML
- Onboarding
- Compliance
- RegTech
---
