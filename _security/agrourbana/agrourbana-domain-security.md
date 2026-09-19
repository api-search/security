---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: agrourbana.ag
  spf: true
hosts:
- cert_expires: Nov 21 07:05:39 2026 GMT
  host: www.agrourbana.ag
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Agrourbana Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AgroUrbana, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: AgroUrbana
provider_slug: agrourbana
slug: agrourbana-domain-security
source_filename: agrourbana-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.agrourbana.ag\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 07:05:39 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: agrourbana.ag\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agrourbana/refs/heads/main/security/agrourbana-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Agriculture
- AgTech
- Vertical Farming
- Food and Beverage
- Controlled Environment Agriculture
- Chile
- Latin America
- Sustainability
---
