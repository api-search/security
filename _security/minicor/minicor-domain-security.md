---
api_specs:
- filename: minicor-openapi.json
  format: json
  label: Laminar API
  slug: laminar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/minicor/refs/heads/main/openapi/minicor-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: laminar.run
  spf: true
hosts:
- cert_expires: Oct 15 22:44:07 2026 GMT
  host: docs.laminar.run
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 15:35:26 2026 GMT
  host: api.laminar.run
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Minicor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Minicor, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Minicor
provider_slug: minicor
slug: minicor-domain-security
source_filename: minicor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.laminar.run\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 22:44:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.laminar.run\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 15:35:26 2026 GMT\n  hsts: null\ndomains:\n- domain: laminar.run\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/minicor/refs/heads/main/security/minicor-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Desktop Automation
- RPA
- Computer Use Agents
- Workflow Automation
- Healthcare
- Legacy Systems
- AI Agents
- Integration
---
