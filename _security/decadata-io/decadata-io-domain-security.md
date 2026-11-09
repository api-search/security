---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: decadata.io
  spf: false
hosts:
- cert_expires: Jan 10 03:15:09 2027 GMT
  host: decadata.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Decadata Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DecaData, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: DecaData
provider_slug: decadata-io
slug: decadata-io-domain-security
source_filename: decadata-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: decadata.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 03:15:09 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: decadata.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/decadata-io/security/decadata-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Data
- Analytics
- Market Insights
- Real-Time
---
