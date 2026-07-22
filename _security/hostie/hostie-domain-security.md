---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hostie.ai
  spf: true
hosts:
- cert_expires: Sep 17 09:45:38 2026 GMT
  host: hostie.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hostie Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hostie, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Hostie
provider_slug: hostie
slug: hostie-domain-security
source_filename: hostie-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hostie.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 09:45:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hostie.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hostie/refs/heads/main/security/hostie-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Restaurants
- Hospitality
- Conversational AI
- Voice AI
- Guest Communication
- Reservations
- Restaurant Technology
---
