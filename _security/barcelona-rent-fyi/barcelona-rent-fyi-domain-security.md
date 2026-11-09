---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: barcelona-rent.fyi
  spf: true
hosts:
- cert_expires: Dec 26 03:45:13 2026 GMT
  host: barcelona-rent.fyi
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Barcelona Rent Fyi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Barcelona Rent, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Barcelona Rent
provider_slug: barcelona-rent-fyi
slug: barcelona-rent-fyi-domain-security
source_filename: barcelona-rent-fyi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: barcelona-rent.fyi\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 03:45:13 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: barcelona-rent.fyi\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/barcelona-rent-fyi/security/barcelona-rent-fyi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Real Estate
- Data
- Housing
- Spain
- Barcelona
- Rentals
---
