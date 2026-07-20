---
api_specs:
- filename: brainfish-public-api-openapi-original.json
  format: json
  label: Brainfish Public API
  slug: brainfish-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brainfish/refs/heads/main/openapi/brainfish-public-api-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: brainfishai.com
  spf: true
hosts:
- cert_expires: Aug 17 18:27:10 2026 GMT
  host: brainfishai.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Brainfish Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Brainfish, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Brainfish
provider_slug: brainfish
slug: brainfish-domain-security
source_filename: brainfish-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: brainfishai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 18:27:10 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: brainfishai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brainfish/refs/heads/main/security/brainfish-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- Customer Support
- Knowledge Base
- Help Desk
- Agents
- Support Automation
- SaaS
---
