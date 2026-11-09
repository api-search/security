---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bloomyesim.com
  spf: true
hosts:
- cert_expires: Jan  6 08:08:43 2027 GMT
  host: bloomyesim.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bloomyesim Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bloomy eSIM, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Bloomy eSIM
provider_slug: bloomyesim-com
slug: bloomyesim-com-domain-security
source_filename: bloomyesim-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bloomyesim.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 08:08:43 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: bloomyesim.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/bloomyesim-com/security/bloomyesim-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- eSIM
- Travel
- Telecommunications
- Japan
- Comparison
---
