---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dns_aid:
    checked: '2026-11-26'
    published: false
  dnssec: false
  domain: tally.markets
  spf: true
hosts:
- cert_expires: Jan 16 04:09:50 2027 GMT
  host: tally.markets
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Tally Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tally, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Tally
provider_slug: tally-markets
slug: tally-markets-domain-security
source_filename: tally-markets-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tally.markets\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 04:09:50 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: tally.markets\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n  dns_aid:\n    checked: '2026-11-26'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/tally-markets/security/tally-markets-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Trading
- AI
---
