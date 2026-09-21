---
api_specs:
- filename: muj428-com-trust-layer-openapi.json
  format: json
  label: MUJ428 Trust Layer API
  slug: muj428-trust-layer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/muj428-com/refs/heads/main/openapi/muj428-com-trust-layer-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: muj428.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: supabase.co
  spf: true
hosts:
- cert_expires: Nov 11 23:11:39 2026 GMT
  host: agents.muj428.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov 24 12:15:45 2026 GMT
  host: wepmhfjzckclvywolrek.supabase.co
  hsts: null
  https: true
  tls_version: TLSv1.2
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Muj428 Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MUJ428 LLC, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: MUJ428 LLC
provider_slug: muj428-com
slug: muj428-com-domain-security
source_filename: muj428-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agents.muj428.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 11 23:11:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: wepmhfjzckclvywolrek.supabase.co\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 24 12:15:45 2026 GMT\n  hsts: null\ndomains:\n- domain: muj428.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: supabase.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/muj428-com/refs/heads/main/security/muj428-com-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Agents
- Agent Trust
- Agentic Commerce
- A2A
- MCP
- x402
- Payments
- Risk
- Verification
- agent-native
---
