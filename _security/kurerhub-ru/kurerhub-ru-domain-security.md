---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: kurerhub.ru
  spf: true
hosts:
- cert_expires: Feb  4 09:51:56 2027 GMT
  host: kurerhub.ru
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: КурьерHUB Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for КурьерHUB, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: КурьерHUB
provider_slug: kurerhub-ru
slug: kurerhub-ru-domain-security
source_filename: kurerhub-ru-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kurerhub.ru\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 09:51:56 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: kurerhub.ru\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/kurerhub-ru/security/kurerhub-ru-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Couriers
- Comparison
- Delivery
- Russia
- Services
---
