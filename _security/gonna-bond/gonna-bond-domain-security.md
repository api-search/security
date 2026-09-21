---
api_specs:
- filename: gonna-bond-legit-openapi.yml
  format: yaml
  label: LEGIT Trust API
  slug: legit-trust-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gonna-bond/refs/heads/main/openapi/gonna-bond-legit-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gonna.bond
  spf: true
hosts:
- cert_expires: Feb  7 13:19:43 2027 GMT
  host: gonna.bond
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  2 22:29:55 2026 GMT
  host: legit.gonna.bond
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Gonna Bond Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GONNA, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: GONNA
provider_slug: gonna-bond
slug: gonna-bond-domain-security
source_filename: gonna-bond-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gonna.bond\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  7 13:19:43 2027 GMT\n  hsts: false\n- host: legit.gonna.bond\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 22:29:55 2026 GMT\n  hsts: null\ndomains:\n- domain: gonna.bond\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gonna-bond/refs/heads/main/security/gonna-bond-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Agents
- Agentic Commerce
- x402
- Trust
- Merchant Trust
- MCP
- A2A
- Algorand
- Blockchain
- Payments
- agent-native
---
