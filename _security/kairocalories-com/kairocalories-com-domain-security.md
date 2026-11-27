---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kairocalories.com
  spf: true
hosts:
- cert_expires: Feb  2 18:33:59 2027 GMT
  host: kairocalories.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Kairo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kairo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Kairo
provider_slug: kairocalories-com
slug: kairocalories-com-domain-security
source_filename: kairocalories-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kairocalories.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  2 18:33:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: kairocalories.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/kairocalories-com/security/kairocalories-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Health
- Nutrition
- Artificial Intelligence
- Mobile App
- Fitness
---
