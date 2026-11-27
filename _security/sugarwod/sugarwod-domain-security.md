---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sugarwod.com
  spf: true
hosts:
- cert_expires: Apr 28 23:59:59 2027 GMT
  host: sugarwod.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: SugarWOD Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SugarWOD, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SugarWOD
provider_slug: sugarwod
slug: sugarwod-domain-security
source_filename: sugarwod-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sugarwod.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Apr 28 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: sugarwod.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/sugarwod/security/sugarwod-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Fitness
- Software-as-a-Service
- Workouts
- Gym Management
- Mobile App
---
