---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: 123loadboard.com
  spf: true
hosts:
- cert_expires: Jan 11 23:59:59 2027 GMT
  host: 123loadboard.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: 123Loadboard Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 123Loadboard, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: 123Loadboard
provider_slug: 123loadboard
slug: 123loadboard-domain-security
source_filename: 123loadboard-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 123loadboard.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 11 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: 123loadboard.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/123loadboard/security/123loadboard-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Freight
- Marketplace
- Logistics
- Load Board
- Transportation
---
