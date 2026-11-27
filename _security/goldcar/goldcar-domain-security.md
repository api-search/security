---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: goldcar.com
  spf: true
hosts:
- cert_expires: Jan 26 08:20:30 2027 GMT
  host: www.goldcar.com
  hsts: true
  hsts_max_age: 600
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Goldcar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Goldcar, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Goldcar
provider_slug: goldcar
slug: goldcar-domain-security
source_filename: goldcar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.goldcar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 08:20:30 2027 GMT\n  hsts: true\n  hsts_max_age: 600\ndomains:\n- domain: goldcar.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/goldcar/security/goldcar-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Car Rental
- Travel
- Europe
- Automotive
- Hospitality
- Company
---
