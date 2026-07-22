---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: plancraft.com
  spf: true
hosts:
- cert_expires: Sep 11 05:28:35 2026 GMT
  host: plancraft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Plancraft Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for plancraft, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: plancraft
provider_slug: plancraft
slug: plancraft-domain-security
source_filename: plancraft-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: plancraft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 05:28:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: plancraft.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plancraft/refs/heads/main/security/plancraft-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- SaaS
- Construction
- Trades
- Handwerk
- Field Service
- Invoicing
- Project Management
- Germany
---
