---
description: ''
domains:
- caa: []
  dmarc: true
  dnssec: true
  domain: evreka.co
  spf: true
hosts:
- cert_expires: Sep 18 11:34:45 2026 GMT
  host: evreka.co
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Evreka Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Evreka, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present.'
provider_name: Evreka
provider_slug: evreka
slug: evreka-domain-security
source_filename: evreka-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: evreka.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 11:34:45 2026 GMT\n  hsts: false\ndomains:\n- domain: evreka.co\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/evreka/refs/heads/main/security/evreka-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Waste Management
- Recycling
- Sustainability
- IoT
- Fleet Management
- Route Optimization
- Environmental
- SaaS
- Asset Management
---
