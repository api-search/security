---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: agentbox.com.au
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: agentboxcrm.com.au
  spf: true
hosts:
- cert_expires: Sep  4 06:29:19 2026 GMT
  host: www.agentbox.com.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  9 23:59:59 2027 GMT
  host: api.agentboxcrm.com.au
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Agentbox Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agentbox, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Agentbox
provider_slug: agentbox
slug: agentbox-domain-security
source_filename: agentbox-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.agentbox.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 06:29:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.agentboxcrm.com.au\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  9 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: agentbox.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: agentboxcrm.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agentbox/refs/heads/main/security/agentbox-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Real-Estate
- Australia
- Property Listings
- PropTech
- CRM
- REAXML
- Portal Feeds
- Rentals
- Commercial Real Estate
- New Zealand
---
