---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: luxembourg-mcp.com
  spf: true
hosts:
- cert_expires: Feb  4 17:17:57 2027 GMT
  host: luxembourg-mcp.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Luxembourg MCP Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Luxembourg MCP, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Luxembourg MCP
provider_slug: luxembourg-mcp-com
slug: luxembourg-mcp-com-domain-security
source_filename: luxembourg-mcp-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: luxembourg-mcp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 17:17:57 2027 GMT\n  hsts: false\ndomains:\n- domain: luxembourg-mcp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/luxembourg-mcp-com/security/luxembourg-mcp-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
