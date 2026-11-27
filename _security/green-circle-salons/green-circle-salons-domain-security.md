---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: greencirclesalons.com
  spf: true
hosts:
- cert_expires: Feb  4 16:04:40 2027 GMT
  host: greencirclesalons.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Green Circle Salons Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Green Circle Salons, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Green Circle Salons
provider_slug: green-circle-salons
slug: green-circle-salons-domain-security
source_filename: green-circle-salons-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: greencirclesalons.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 16:04:40 2027 GMT\n  hsts: false\ndomains:\n- domain: greencirclesalons.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/green-circle-salons/security/green-circle-salons-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Sustainability
- Beauty
- Salon
- Environment
- Waste Reduction
---
