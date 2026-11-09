---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: dev-match.xyz
  spf: true
hosts:
- cert_expires: Jan 11 14:19:13 2027 GMT
  host: dev-match.xyz
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dev Match Xyz Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DevMatch, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: DevMatch
provider_slug: dev-match-xyz
slug: dev-match-xyz-domain-security
source_filename: dev-match-xyz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dev-match.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 14:19:13 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: dev-match.xyz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/dev-match-xyz/security/dev-match-xyz-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Engineering
- Hiring
- Deep Tech
- Artificial Intelligence
- Platform
---
