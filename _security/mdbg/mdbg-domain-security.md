---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mdbg.net
  spf: true
hosts:
- cert_expires: Jan  4 13:58:02 2027 GMT
  host: mdbg.net
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mdbg Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MDBG Chinese Dictionary, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: MDBG Chinese Dictionary
provider_slug: mdbg
slug: mdbg-domain-security
source_filename: mdbg-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mdbg.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 13:58:02 2027 GMT\n  hsts: true\n  hsts_max_age: 86400\ndomains:\n- domain: mdbg.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/mdbg/security/mdbg-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Chinese
- Dictionary
- Language-Learning
- Education
---
