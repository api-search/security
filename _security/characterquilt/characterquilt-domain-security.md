---
api_specs:
- filename: characterquilt-branding-openapi.yml
  format: yaml
  label: CharacterQuilt Brand Profiles
  slug: characterquilt-brand-profiles
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/characterquilt/refs/heads/main/openapi/characterquilt-branding-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: characterquilt.com
  spf: true
hosts:
- cert_expires: Sep 27 08:58:48 2026 GMT
  host: www.characterquilt.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Characterquilt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CharacterQuilt, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: CharacterQuilt
provider_slug: characterquilt
slug: characterquilt-domain-security
source_filename: characterquilt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.characterquilt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 08:58:48 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: characterquilt.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/characterquilt/refs/heads/main/security/characterquilt-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Marketing
- Artificial Intelligence
- AI Agents
- Marketing Automation
- Campaign Management
- Brand Identity
- Computer Use Agents
- Y Combinator
- Data
---
