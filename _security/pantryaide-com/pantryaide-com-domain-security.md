---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: pantryaide.com
  spf: false
hosts:
- cert_expires: Jan 26 16:10:51 2027 GMT
  host: pantryaide.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Pantry Aide Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pantry Aide, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Pantry Aide
provider_slug: pantryaide-com
slug: pantryaide-com-domain-security
source_filename: pantryaide-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pantryaide.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 16:10:51 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: pantryaide.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/pantryaide-com/security/pantryaide-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Meal Planning
- Grocery Shopping
- Artificial Intelligence
- Free Tier
- Paid Plans
---
