---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: letmeship.com
  spf: true
hosts:
- cert_expires: Jan 22 10:20:29 2027 GMT
  host: letmeship.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Letmeship Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LetMeShip, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: LetMeShip
provider_slug: letmeship
slug: letmeship-domain-security
source_filename: letmeship-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: letmeship.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 10:20:29 2027 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: letmeship.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/letmeship/security/letmeship-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Shipping
- Logistics
- B2B
- API
- Europe
---
