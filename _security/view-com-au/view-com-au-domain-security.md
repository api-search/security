---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: view.com.au
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: viewmediagroup.com.au
  spf: true
hosts:
- cert_expires: Nov  8 23:59:59 2026 GMT
  host: view.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 06:25:25 2026 GMT
  host: www.viewmediagroup.com.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug  4 06:28:13 2026 GMT
  host: mcp.view.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: View Com Au Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for View.com.au, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: View.com.au
provider_slug: view-com-au
slug: view-com-au-domain-security
source_filename: view-com-au-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: view.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 23:59:59 2026 GMT\n  hsts: null\n- host: www.viewmediagroup.com.au\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 12 06:25:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: mcp.view.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  4 06:28:13 2026 GMT\n  hsts: null\ndomains:\n- domain: view.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: viewmediagroup.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/view-com-au/refs/heads/main/security/view-com-au-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Real-Estate
- Australia
- Property Listings
- Property Portal
- PropTech
- Rentals
- Off-Market Property Data
- MCP
- agent-native
---
