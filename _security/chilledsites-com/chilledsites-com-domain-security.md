---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: chilledsites.com
  spf: false
hosts:
- cert_expires: Oct 19 19:18:26 2026 GMT
  host: chilledsites.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Chilledsites Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ChilledSites, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: ChilledSites
provider_slug: chilledsites-com
slug: chilledsites-com-domain-security
source_filename: chilledsites-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: chilledsites.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 19:18:26 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: chilledsites.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chilledsites-com/refs/heads/main/security/chilledsites-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Website Builder
- Artificial Intelligence
- No-Code
- Web Hosting
- Image Generation
- Video Generation
- Advertising
- MCP
- Agents
- A2A
- Small Business
- United Kingdom
---
