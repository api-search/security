---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: chickin.id
  spf: true
hosts:
- cert_expires: Sep 30 01:58:37 2026 GMT
  host: chickin.id
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Chickin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chickin, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Chickin
provider_slug: chickin
slug: chickin-domain-security
source_filename: chickin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: chickin.id\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 01:58:37 2026 GMT\n  hsts: false\ndomains:\n- domain: chickin.id\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chickin/refs/heads/main/security/chickin-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Poultry
- Agriculture
- AgTech
- IoT
- Smart Farming
- Supply Chain
- Livestock
- Indonesia
---
