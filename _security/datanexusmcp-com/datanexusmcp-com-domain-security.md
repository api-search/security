---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: datanexusmcp.com
  spf: true
hosts:
- cert_expires: Jan 22 07:21:54 2027 GMT
  host: datanexusmcp.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: DataNexus MCP Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DataNexus MCP, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: DataNexus MCP
provider_slug: datanexusmcp-com
slug: datanexusmcp-com-domain-security
source_filename: datanexusmcp-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: datanexusmcp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 07:21:54 2027 GMT\n  hsts: false\ndomains:\n- domain: datanexusmcp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/datanexusmcp-com/security/datanexusmcp-com-domain-security.yml
summary_line: TLSv1.3
tags:
- Data Intelligence
- AI Integration
- Public Data
- Tools
- Compliance
- Non-Profit
---
