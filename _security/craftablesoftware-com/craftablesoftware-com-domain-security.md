---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: craftablesoftware.com
  spf: true
hosts:
- cert_expires: Apr 23 23:59:59 2027 GMT
  host: craftablesoftware.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: mcp.craftablesoftware.com
  https: false
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: craftable software Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for craftable software, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: craftable software
provider_slug: craftablesoftware-com
slug: craftablesoftware-com-domain-security
source_filename: craftablesoftware-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: craftablesoftware.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 23 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: mcp.craftablesoftware.com\n  https: false\ndomains:\n- domain: craftablesoftware.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/craftablesoftware-com/security/craftablesoftware-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Software Development
- Artificial Intelligence
- Consulting
- Legacy Modernization
- MCP
- Portugal
---
