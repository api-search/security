---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: supercharge.bingo
  spf: true
hosts:
- cert_expires: Jan 17 03:01:51 2027 GMT
  host: supercharge.bingo
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Supercharge Bingo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for supercharge.bingo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: supercharge.bingo
provider_slug: supercharge-bingo
slug: supercharge-bingo-domain-security
source_filename: supercharge-bingo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: supercharge.bingo\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 03:01:51 2027 GMT\n  hsts: false\ndomains:\n- domain: supercharge.bingo\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/supercharge-bingo/security/supercharge-bingo-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Gaming
- EV
- Community
- Tesla
---
