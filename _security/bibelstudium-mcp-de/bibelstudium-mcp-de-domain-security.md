---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bibelstudium-mcp.de
  spf: true
hosts:
- cert_expires: Dec 22 21:14:31 2026 GMT
  host: bibelstudium-mcp.de
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bibelstudium MCP Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bibelstudium MCP, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Bibelstudium MCP
provider_slug: bibelstudium-mcp-de
slug: bibelstudium-mcp-de-domain-security
source_filename: bibelstudium-mcp-de-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bibelstudium-mcp.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 21:14:31 2026 GMT\n  hsts: false\ndomains:\n- domain: bibelstudium-mcp.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/bibelstudium-mcp-de/security/bibelstudium-mcp-de-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Bible
---
