---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gt.bio
  spf: true
hosts:
- cert_expires: Jan 16 16:15:01 2027 GMT
  host: gt.bio
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Gt Bio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GT Bio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: GT Bio
provider_slug: gt-bio
slug: gt-bio-domain-security
source_filename: gt-bio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gt.bio\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 16:15:01 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: gt.bio\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/gt-bio/security/gt-bio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Biotechnology
- Genetic Medicines
- AI
- Drug Delivery
- Startup
---
