---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: aimailmcp.com
  spf: true
hosts:
- cert_expires: Jan  6 13:05:57 2027 GMT
  host: aimailmcp.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: AI Mail MCP Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AI Mail MCP, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: AI Mail MCP
provider_slug: aimailmcp-com
slug: aimailmcp-com-domain-security
source_filename: aimailmcp-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aimailmcp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 13:05:57 2027 GMT\n  hsts: false\ndomains:\n- domain: aimailmcp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/aimailmcp-com/security/aimailmcp-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Email
- Artificial Intelligence
- MCP
- Software-as-a-Service
- Inbox
---
