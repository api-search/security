---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: forkandgood.com
  spf: true
hosts:
- cert_expires: Nov 28 15:22:51 2026 GMT
  host: forkandgood.com
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fork And Good Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fork & Good, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Fork & Good
provider_slug: fork-and-good
slug: fork-and-good-domain-security
source_filename: fork-and-good-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: forkandgood.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 15:22:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\ndomains:\n- domain: forkandgood.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/fork-and-good/security/fork-and-good-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- FoodTech
- Sustainable
- Biotechnology
- MeatProduction
- ClimateImpact
- Company
---
