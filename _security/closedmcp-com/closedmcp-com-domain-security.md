---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: closedmcp.com
  spf: false
hosts:
- cert_expires: Jan 10 16:07:21 2027 GMT
  host: closedmcp.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ClosedMCP Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ClosedMCP, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: ClosedMCP
provider_slug: closedmcp-com
slug: closedmcp-com-domain-security
source_filename: closedmcp-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: closedmcp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 16:07:21 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: closedmcp.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/closedmcp-com/security/closedmcp-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- MCP
- AI Agents
- Gateways
- Access Control
- Serverless
- Developer Tools
---
