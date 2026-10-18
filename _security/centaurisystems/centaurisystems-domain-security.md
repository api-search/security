---
api_specs:
- filename: centaurisystems-oauth-api-openapi.yml
  format: yaml
  label: Centauri Systems OAuth API
  slug: centaurisystems-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centaurisystems/refs/heads/main/openapi/centaurisystems-oauth-api-openapi.yml
- filename: centaurisystems-payments-api-openapi.yml
  format: yaml
  label: Centauri Systems Payments API
  slug: centaurisystems-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centaurisystems/refs/heads/main/openapi/centaurisystems-payments-api-openapi.yml
- filename: centaurisystems-users-api-openapi.yml
  format: yaml
  label: Centauri Systems Users API
  slug: centaurisystems-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centaurisystems/refs/heads/main/openapi/centaurisystems-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: centaurisystems.io
  spf: true
hosts:
- cert_expires: Nov 18 18:03:47 2026 GMT
  host: centaurisystems.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Centaurisystems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Centauri Systems, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Centauri Systems
provider_slug: centaurisystems
slug: centaurisystems-domain-security
source_filename: centaurisystems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: centaurisystems.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 18 18:03:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: centaurisystems.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/centaurisystems/refs/heads/main/security/centaurisystems-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Developer-Portal
- API-Tooling
- Apigee
- Cloud-Platform
---
