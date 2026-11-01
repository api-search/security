---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tradebasis.net
  spf: false
hosts:
- cert_expires: Dec  5 00:52:54 2026 GMT
  host: tradebasis.net
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Tradebasis Net Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for tradebasis-net, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: tradebasis-net
provider_slug: tradebasis-net
slug: tradebasis-net-domain-security
source_filename: tradebasis-net-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tradebasis.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 00:52:54 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: tradebasis.net\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/tradebasis-net/security/tradebasis-net-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Automotive
- Software
- Appraisal
- Used Vehicles
---
