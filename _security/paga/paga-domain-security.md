---
api_specs:
- filename: paga-openapi.yml
  format: yaml
  label: Paga Collect API
  slug: paga-collect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paga/refs/heads/main/openapi/paga-openapi.yml
- filename: paga-openapi.yml
  format: yaml
  label: Paga Business API
  slug: paga-business-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paga/refs/heads/main/openapi/paga-openapi.yml
- filename: paga-openapi.yml
  format: yaml
  label: Paga Direct Debit API
  slug: paga-direct-debit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paga/refs/heads/main/openapi/paga-openapi.yml
description: ''
domains: []
hosts:
- cert_expires: Dec 12 13:07:15 2026 GMT
  host: www.paga.com
  http_status: 302
  https: true
  tls_verified: true
- cert_expires: Oct  2 11:33:03 2026 GMT
  host: developer-docs.paga.com
  http_status: 302
  https: true
  tls_verified: true
- cert_expires: Dec 12 13:07:15 2026 GMT
  host: collect.paga.com
  http_status: 403
  https: true
  notes: Collect API host; 403 to unauthenticated browser GET is expected (API POST endpoints only).
  tls_verified: true
- cert_expires: Sep 29 12:13:50 2026 GMT
  host: www.mypaga.com
  http_status: 200
  https: true
  notes: Business API host (path /paga-webservices/business-rest/secured).
  tls_verified: true
kind: domain-security
layout: security
method: probed
name: Paga Domain Security
name_suffix: Domain Security
overview: Domain security posture for Paga, probed live across 4 host(s) and 0 registrable domain(s). 4 host(s) serve HTTPS; 0 advertise HSTS.
provider_name: Paga
provider_slug: paga
slug: paga-domain-security
source_filename: paga-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live TLS/HTTP probes of apis.yml + OpenAPI hosts (2026-07-17)\nhosts:\n- host: www.paga.com\n  https: true\n  http_status: 302\n  tls_verified: true\n  cert_expires: Dec 12 13:07:15 2026 GMT\n- host: developer-docs.paga.com\n  https: true\n  http_status: 302\n  tls_verified: true\n  cert_expires: Oct  2 11:33:03 2026 GMT\n- host: collect.paga.com\n  https: true\n  http_status: 403\n  tls_verified: true\n  cert_expires: Dec 12 13:07:15 2026 GMT\n  notes: Collect API host; 403 to unauthenticated browser GET is expected (API POST endpoints only).\n- host: www.mypaga.com\n  https: true\n  http_status: 200\n  tls_verified: true\n  cert_expires: Sep 29 12:13:50 2026 GMT\n  notes: Business API host (path /paga-webservices/business-rest/secured).\ntransport:\n- All documented endpoints are HTTPS only.\n- Business API additionally requires caller IP whitelisting before access is granted.\n- Per-request payload integrity is enforced by\
  \ a SHA-512 hash header over ordered request parameters plus the account hash key.\nnotes: >-\n  All four in-scope hosts terminate valid TLS certificates. Region hosts are\n  Nigeria-oriented (mypaga.com for the Business API, collect.paga.com for\n  Collect and Direct Debit). No formal Paga security.txt was confirmed at probe\n  time; report vulnerabilities to Paga support.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paga/refs/heads/main/security/paga-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Payments
- Mobile Money
- Fintech
- Collections
- Nigeria
---
