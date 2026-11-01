---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: gv.at
  spf: false
hosts:
- cert_expires: Apr 29 23:59:59 2027 GMT
  host: www.wien.gv.at
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: City Of Vienna Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for City of Vienna, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: City of Vienna
provider_slug: city-of-vienna
slug: city-of-vienna-domain-security
source_filename: city-of-vienna-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wien.gv.at\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 29 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: gv.at\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/city-of-vienna/security/city-of-vienna-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
---
