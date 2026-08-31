---
api_specs:
- filename: palenca-vech-admin-api-openapi.yml
  format: yaml
  label: Palenca (Vech) admin API
  slug: palenca-vech-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/palenca-vech/refs/heads/main/openapi/palenca-vech-admin-api-openapi.yml
- filename: palenca-vech-check-platform-health-api-openapi.yml
  format: yaml
  label: Palenca (Vech) Check Platform Health API
  slug: palenca-vech-check-platform-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/palenca-vech/refs/heads/main/openapi/palenca-vech-check-platform-health-api-openapi.yml
- filename: palenca-vech-console-api-openapi.yml
  format: yaml
  label: Palenca (Vech) console API
  slug: palenca-vech-console-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/palenca-vech/refs/heads/main/openapi/palenca-vech-console-api-openapi.yml
- filename: palenca-vech-ping-api-openapi.yml
  format: yaml
  label: Palenca (Vech) Ping API
  slug: palenca-vech-ping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/palenca-vech/refs/heads/main/openapi/palenca-vech-ping-api-openapi.yml
- filename: palenca-vech-pong-api-openapi.yml
  format: yaml
  label: Palenca (Vech) Pong API
  slug: palenca-vech-pong-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/palenca-vech/refs/heads/main/openapi/palenca-vech-pong-api-openapi.yml
- filename: palenca-vech-v1-api-openapi.yml
  format: yaml
  label: Palenca (Vech) v1 API
  slug: palenca-vech-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/palenca-vech/refs/heads/main/openapi/palenca-vech-v1-api-openapi.yml
- filename: palenca-vech-version-api-openapi.yml
  format: yaml
  label: Palenca (Vech) Version API
  slug: palenca-vech-version-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/palenca-vech/refs/heads/main/openapi/palenca-vech-version-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: palenca.com
  spf: true
hosts:
- cert_expires: Sep  5 20:30:57 2026 GMT
  host: palenca.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Palenca Vech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Palenca (Vech), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Palenca (Vech)
provider_slug: palenca-vech
slug: palenca-vech-domain-security
source_filename: palenca-vech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: palenca.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 20:30:57 2026 GMT\n  hsts: null\ndomains:\n- domain: palenca.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/palenca-vech/refs/heads/main/security/palenca-vech-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Income Verification
- Employment Verification
- Fintech
- Gig Economy
- Latin America
- Identity
---
