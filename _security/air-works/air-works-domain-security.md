---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: airworks.aero
  spf: false
hosts:
- cert_expires: Jan  8 06:51:36 2027 GMT
  host: airworks.aero
  hsts: true
  hsts_max_age: 10886400
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Air Works Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Air Works, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: Air Works
provider_slug: air-works
slug: air-works-domain-security
source_filename: air-works-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: airworks.aero\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  8 06:51:36 2027 GMT\n  hsts: true\n  hsts_max_age: 10886400\ndomains:\n- domain: airworks.aero\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/air-works/security/air-works-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Aviation
- MRO
- Maintenance
- India
- Services
---
