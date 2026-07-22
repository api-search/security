---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: draftea.mx
  spf: false
hosts:
- cert_expires: Sep 11 16:09:04 2026 GMT
  host: www.draftea.mx
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Draftea Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Draftea, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Draftea
provider_slug: draftea
slug: draftea-domain-security
source_filename: draftea-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.draftea.mx\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 16:09:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: draftea.mx\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/draftea/refs/heads/main/security/draftea-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Fantasy Sports
- Daily Fantasy Sports
- Sports Betting
- Gaming
- Sports
- Mexico
- Latin America
- Consumer
---
