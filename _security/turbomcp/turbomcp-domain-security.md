---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: turbomcp.ai
  spf: false
hosts:
- cert_expires: Jan  5 07:05:58 2027 GMT
  host: turbomcp.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Turbomcp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Turbo MCP, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Turbo MCP
provider_slug: turbomcp
slug: turbomcp-domain-security
source_filename: turbomcp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: turbomcp.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 07:05:58 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: turbomcp.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/turbomcp/security/turbomcp-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Artificial Intelligence
- Management
- Control Plane
- Self-Hosted
---
