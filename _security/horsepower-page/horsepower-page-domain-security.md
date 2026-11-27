---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: horsepower.page
  spf: true
hosts:
- cert_expires: Feb 28 23:59:59 2027 GMT
  host: horsepower.page
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Horsepower Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Horsepower, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Horsepower
provider_slug: horsepower-page
slug: horsepower-page-domain-security
source_filename: horsepower-page-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: horsepower.page\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 28 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: horsepower.page\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/horsepower-page/security/horsepower-page-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- StableManagement
- YardSoftware
- HorseOwners
- Free Tier
---
