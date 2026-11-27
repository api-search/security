---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: elron.club
  spf: true
hosts:
- cert_expires: Jan 14 13:58:48 2027 GMT
  host: elron.club
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Elron Club Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Elron Club, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Elron Club
provider_slug: elron-club
slug: elron-club-domain-security
source_filename: elron-club-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: elron.club\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 13:58:48 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: elron.club\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/elron-club/security/elron-club-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Real Estate
- Housing
- Rentals
- Switzerland
- Furnished
---
