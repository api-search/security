---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ryanair.com
  spf: true
hosts:
- cert_expires: Feb 17 23:59:59 2027 GMT
  host: ryanair.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ryanair Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ryanair, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Ryanair
provider_slug: ryanair
slug: ryanair-domain-security
source_filename: ryanair-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ryanair.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 17 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ryanair.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ryanair/refs/heads/main/security/ryanair-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Airline
- Travel
- Europe
- LowCost
---
