---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: cortex-gateway.dev
  spf: true
hosts:
- cert_expires: Jan 31 02:50:35 2027 GMT
  host: cortex-gateway.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cortex Gateway Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cortex Gateway, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Cortex Gateway
provider_slug: cortex-gateway-dev
slug: cortex-gateway-dev-domain-security
source_filename: cortex-gateway-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cortex-gateway.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 02:50:35 2027 GMT\n  hsts: false\ndomains:\n- domain: cortex-gateway.dev\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/cortex-gateway-dev/security/cortex-gateway-dev-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- MCP
- MCP Gateway
- Open Source
- OAuth 2.1
- AI Agents
- Identity
- Authorization
- Self-Hosted
---
