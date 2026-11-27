---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: likarika.se
  spf: true
hosts:
- cert_expires: Feb 11 07:32:17 2027 GMT
  host: likarika.se
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Lika Rika Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lika Rika, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Lika Rika
provider_slug: likarika-se
slug: likarika-se-domain-security
source_filename: likarika-se-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: likarika.se\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 11 07:32:17 2027 GMT\n  hsts: false\ndomains:\n- domain: likarika.se\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/likarika-se/security/likarika-se-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Finance
- Household
- Budgeting
- ExpenseSharing
- Sweden
---
