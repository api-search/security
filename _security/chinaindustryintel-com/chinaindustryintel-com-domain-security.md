---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: chinaindustryintel.com
  spf: true
hosts:
- cert_expires: Jan 16 18:09:06 2027 GMT
  host: chinaindustryintel.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 16 18:09:06 2027 GMT
  host: mcp.chinaindustryintel.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: China Industry Intel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for China Industry Intel, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: China Industry Intel
provider_slug: chinaindustryintel-com
slug: chinaindustryintel-com-domain-security
source_filename: chinaindustryintel-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: chinaindustryintel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 18:09:06 2027 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: mcp.chinaindustryintel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 18:09:06 2027 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: chinaindustryintel.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/chinaindustryintel-com/security/chinaindustryintel-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- China
- Industry Intelligence
- Media
- Market Research
- Supply Chain
- MCP
---
