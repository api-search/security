---
api_specs:
- filename: apimesh-xyz-openapi.yml
  format: yaml
  label: APIMesh Web Analysis APIs
  slug: apimesh-web-analysis-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apimesh-xyz/refs/heads/main/openapi/apimesh-xyz-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: apimesh.xyz
  spf: false
hosts:
- cert_expires: Nov 25 02:35:33 2026 GMT
  host: apimesh.xyz
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 25 22:35:39 2026 GMT
  host: agentsmd.apimesh.xyz
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 25 22:35:39 2026 GMT
  host: stripesig.apimesh.xyz
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Apimesh Xyz Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for APIMesh, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: APIMesh
provider_slug: apimesh-xyz
slug: apimesh-xyz-domain-security
source_filename: apimesh-xyz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apimesh.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 02:35:33 2026 GMT\n  hsts: false\n- host: agentsmd.apimesh.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 22:35:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: stripesig.apimesh.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 22:35:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: apimesh.xyz\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apimesh-xyz/refs/heads/main/security/apimesh-xyz-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Web Analysis
- SEO
- Web Security
- Email Verification
- Developer Tools
- Micropayments
- x402
- MCP
- Agent-Native
- Webhook
- AI Coding Agents
- Open Source
- A2A
---
