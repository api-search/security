---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tyb.xyz
  spf: true
hosts:
- cert_expires: Jan 27 13:17:29 2027 GMT
  host: www.tyb.xyz
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Tyb Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TYB, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: TYB
provider_slug: tyb
slug: tyb-domain-security
source_filename: tyb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tyb.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 13:17:29 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tyb.xyz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/tyb/security/tyb-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Rewards
- Community
- Engagement
- Platform
---
