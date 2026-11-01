---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: easyweek.io
  spf: true
hosts:
- cert_expires: Jan 19 16:48:33 2027 GMT
  host: easyweek.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Easyweek Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for easyweek-io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: easyweek-io
provider_slug: easyweek-io
slug: easyweek-io-domain-security
source_filename: easyweek-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: easyweek.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 19 16:48:33 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: easyweek.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/easyweek-io/security/easyweek-io-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Marketplace
- Booking
- Services
- US
- Consumer
---
