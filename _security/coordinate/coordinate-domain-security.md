---
api_specs:
- filename: coordinate-openapi.yml
  format: yaml
  label: Coordinate REST API
  slug: coordinate-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coordinate/refs/heads/main/openapi/coordinate-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: coordinatehq.com
  spf: true
hosts:
- cert_expires: Oct  1 07:48:56 2026 GMT
  host: coordinatehq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Coordinate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Coordinate, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Coordinate
provider_slug: coordinate
slug: coordinate-domain-security
source_filename: coordinate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: coordinatehq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 07:48:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: coordinatehq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coordinate/refs/heads/main/security/coordinate-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Enterprise Saas
- Project Management
- Client Portal
- Client Onboarding
- Professional Services
- Workflow Automation
- Collaboration
- Webhooks
---
