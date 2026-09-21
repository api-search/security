---
api_specs:
- filename: getminds-openapi.json
  format: json
  label: Minds Public API
  slug: minds-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getminds/refs/heads/main/openapi/getminds-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: getminds.ai
  spf: true
hosts:
- cert_expires: Dec  7 08:26:13 2026 GMT
  host: getminds.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  7 08:26:13 2026 GMT
  host: api.getminds.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Getminds Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Minds, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Minds
provider_slug: getminds
slug: getminds-domain-security
source_filename: getminds-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getminds.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 08:26:13 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.getminds.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 08:26:13 2026 GMT\n  hsts: false\ndomains:\n- domain: getminds.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/getminds/refs/heads/main/security/getminds-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Synthetic Research
- Market Research
- Surveys
- User Research
- Marketing Analytics
- ai-personas
- MCP
- agent-native
- GDPR
---
