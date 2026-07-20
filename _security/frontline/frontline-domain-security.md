---
api_specs:
- filename: frontline-openapi-original.yml
  format: yaml
  label: Frontline Public API
  slug: frontline-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frontline/refs/heads/main/openapi/frontline-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: getfrontline.ai
  spf: true
hosts:
- cert_expires: Oct  6 23:39:15 2026 GMT
  host: getfrontline.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 25 23:59:59 2026 GMT
  host: prod-api.getfrontline.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Frontline Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Frontline, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Frontline
provider_slug: frontline
slug: frontline-domain-security
source_filename: frontline-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getfrontline.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 23:39:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: prod-api.getfrontline.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: getfrontline.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/frontline/refs/heads/main/security/frontline-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- CRM
- AI Agents
- Sales Automation
- Customer Support
- Workflows
- Conversational AI
---
