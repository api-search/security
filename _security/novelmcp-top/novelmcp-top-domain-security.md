---
description: ''
domains:
- caa:
  - novelmcp.top.pages.dnsoe6.com.
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: novelmcp.top
  spf: false
hosts:
- cert_expires: Jan  8 23:59:59 2027 GMT
  host: novelmcp.top
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Novel Factory MCP Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Novel Factory MCP, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=none).'
provider_name: Novel Factory MCP
provider_slug: novelmcp-top
slug: novelmcp-top-domain-security
source_filename: novelmcp-top-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: novelmcp.top\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: novelmcp.top\n  dnssec: true\n  caa:\n  - novelmcp.top.pages.dnsoe6.com.\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/novelmcp-top/security/novelmcp-top-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Writing
- Chinese
- MCP
- Tools
- Free
---
