---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: funcom.com
  spf: true
hosts:
- cert_expires: Oct  2 13:45:36 2026 GMT
  host: www.funcom.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Funcom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Funcom, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Funcom
provider_slug: funcom
slug: funcom-domain-security
source_filename: funcom-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.funcom.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 13:45:36 2026 GMT\n  hsts: false\ndomains:\n- domain: funcom.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/funcom/refs/heads/main/security/funcom-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Consumer
- Video Games
- Game Developer
- Gaming
- Entertainment
- MMO
- Norway
---
