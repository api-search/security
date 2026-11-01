---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: go.id
  spf: false
hosts:
- cert_expires: Mar 20 23:59:59 2027 GMT
  host: bmkg.go.id
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bmkg Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BMKG, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: BMKG
provider_slug: bmkg
slug: bmkg-domain-security
source_filename: bmkg-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bmkg.go.id\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 20 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: go.id\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/bmkg/security/bmkg-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Weather
- Climate
- Geophysics
- Indonesia
---
