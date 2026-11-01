---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: accupedo.com
  spf: true
hosts:
- cert_expires: Jan  5 08:24:58 2027 GMT
  host: accupedo.com
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Accupedo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Accupedo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Accupedo
provider_slug: accupedo
slug: accupedo-domain-security
source_filename: accupedo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: accupedo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 08:24:58 2027 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: accupedo.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/accupedo/security/accupedo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Health
- Fitness
- MobileApp
- Pedometer
---
