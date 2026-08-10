---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: agryco.com
  spf: true
hosts:
- cert_expires: Aug 29 11:53:05 2026 GMT
  host: www.agryco.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Agriconomie Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agryco, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Agryco
provider_slug: agriconomie
slug: agriconomie-domain-security
source_filename: agriconomie-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.agryco.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 11:53:05 2026 GMT\n  hsts: null\ndomains:\n- domain: agryco.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agriconomie/refs/heads/main/security/agriconomie-domain-security.yml
summary_line: TLSv1.3
tags:
- Agriculture
- AgTech
- E-Commerce
- Marketplace
- Farm Supplies
- Agricultural Inputs
- Retail
- France
- Europe
- Company
---
