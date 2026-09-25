---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: aerofarms.com
  spf: false
hosts:
- cert_expires: Nov 13 07:46:21 2026 GMT
  host: www.aerofarms.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aerofarms Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AeroFarms, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: AeroFarms
provider_slug: aerofarms
slug: aerofarms-domain-security
source_filename: aerofarms-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aerofarms.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 07:46:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: aerofarms.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aerofarms/refs/heads/main/security/aerofarms-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Agriculture
- Vertical Farming
- Indoor Farming
- AgTech
- Food and Beverage
- Consumer Packaged Goods
- Microgreens
- Sustainability
- Content
- Commerce
- MCP
---
