---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: atomicreps.com
  spf: true
hosts:
- cert_expires: Jan 30 17:43:14 2027 GMT
  host: atomicreps.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Atomic Reps AB Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Atomic Reps AB, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Atomic Reps AB
provider_slug: atomicreps-com
slug: atomicreps-com-domain-security
source_filename: atomicreps-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: atomicreps.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 17:43:14 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: atomicreps.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/atomicreps-com/security/atomicreps-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Developer Tools
- Education
- Artificial Intelligence
- Software Engineering
- Sweden
---
