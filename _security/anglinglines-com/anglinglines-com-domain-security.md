---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: anglinglines.com
  spf: true
hosts:
- cert_expires: Dec 22 09:33:06 2026 GMT
  host: anglinglines.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Angling Lines Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Angling Lines, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Angling Lines
provider_slug: anglinglines-com
slug: anglinglines-com-domain-security
source_filename: anglinglines-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: anglinglines.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 09:33:06 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: anglinglines.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/anglinglines-com/security/anglinglines-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fishing
- carp
- Holiday
- France
- Angling
---
