---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: micoradar.com
  spf: true
hosts:
- cert_expires: Feb 16 10:12:10 2027 GMT
  host: micoradar.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MicoRadar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MicoRadar, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: MicoRadar
provider_slug: micoradar-com
slug: micoradar-com-domain-security
source_filename: micoradar-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: micoradar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 16 10:12:10 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: micoradar.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/micoradar-com/security/micoradar-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Mushroom
- Forecast
- Spain
- Outdoors
---
