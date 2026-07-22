---
api_specs:
- filename: rhythms-openapi-original.json
  format: json
  label: Rhythms API
  slug: rhythms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rhythms/refs/heads/main/openapi/rhythms-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: rhythms.ai
  spf: true
hosts:
- cert_expires: Sep 20 05:16:10 2026 GMT
  host: www.rhythms.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 10 23:59:59 2026 GMT
  host: api.rhythms.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rhythms Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rhythms, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Rhythms
provider_slug: rhythms
slug: rhythms-domain-security
source_filename: rhythms-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rhythms.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 05:16:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.rhythms.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: rhythms.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rhythms/refs/heads/main/security/rhythms-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai
- Productivity
- Goal Tracking
- OKR
- Workflow Automation
- Team Collaboration
- Business Reviews
- MCP
---
