---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: mspmcp.com
  spf: false
hosts:
- cert_expires: Feb 11 23:19:34 2027 GMT
  host: mspmcp.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Instinct MCP Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Instinct MCP, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Instinct MCP
provider_slug: mspmcp-com
slug: mspmcp-com-domain-security
source_filename: mspmcp-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mspmcp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 11 23:19:34 2027 GMT\n  hsts: false\ndomains:\n- domain: mspmcp.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/mspmcp-com/security/mspmcp-com-domain-security.yml
summary_line: TLSv1.3
tags:
- Artificial Intelligence
- Market Intelligence
- Managed Service
- MSP
- Data Analytics
---
