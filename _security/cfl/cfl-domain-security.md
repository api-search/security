---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cfl.ca
  spf: true
hosts:
- cert_expires: Nov  9 11:48:29 2026 GMT
  host: cfl.ca
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cfl Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CFL scoreboard JSON, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: CFL scoreboard JSON
provider_slug: cfl
slug: cfl-domain-security
source_filename: cfl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cfl.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 11:48:29 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: cfl.ca\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/cfl/security/cfl-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Sports
- Football
- Canada
- ProfessionalLeague
- Entertainment
---
