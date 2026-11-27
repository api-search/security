---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: datagoat.io
  spf: true
hosts:
- cert_expires: Jan 26 18:17:06 2027 GMT
  host: datagoat.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Data Goat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Data Goat, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Data Goat
provider_slug: datagoat-io
slug: datagoat-io-domain-security
source_filename: datagoat-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: datagoat.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 18:17:06 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: datagoat.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/datagoat-io/security/datagoat-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Artificial Intelligence
- Decisions
- Software-as-a-Service
- Analytics
---
