---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: merona.io
  spf: true
hosts:
- cert_expires: Feb 11 22:07:42 2027 GMT
  host: merona.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: merona Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for merona, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: merona
provider_slug: merona-io
slug: merona-io-domain-security
source_filename: merona-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: merona.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 11 22:07:42 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: merona.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/merona-io/security/merona-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Blockchain
- Data
- Trust
- Open Source
---
