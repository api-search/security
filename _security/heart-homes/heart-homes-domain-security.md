---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: heart.homes
  spf: true
hosts:
- cert_expires: Dec 23 18:32:19 2026 GMT
  host: heart.homes
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Heart Homes Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Heart Homes, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Heart Homes
provider_slug: heart-homes
slug: heart-homes-domain-security
source_filename: heart-homes-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: heart.homes\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 18:32:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: heart.homes\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/heart-homes/security/heart-homes-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Real Estate
- Data Analytics
- Dubai
- Property Prices
- Open Data
---
