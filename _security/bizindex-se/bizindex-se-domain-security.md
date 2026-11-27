---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: bizindex.se
  spf: false
hosts:
- cert_expires: Jan  5 23:59:59 2027 GMT
  host: bizindex.se
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bizindex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bizindex, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Bizindex
provider_slug: bizindex-se
slug: bizindex-se-domain-security
source_filename: bizindex-se-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bizindex.se\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: bizindex.se\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/bizindex-se/security/bizindex-se-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Business
- Index
- Swedish
- Companies
- Open Data
---
