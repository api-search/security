---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gastrosync.com
  spf: false
hosts:
- cert_expires: Jan 17 12:08:00 2027 GMT
  host: gastrosync.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Gastrosync Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gastrosync, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Gastrosync
provider_slug: gastrosync-com
slug: gastrosync-com-domain-security
source_filename: gastrosync-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gastrosync.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 12:08:00 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: gastrosync.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/gastrosync-com/security/gastrosync-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Software-as-a-Service
- Gastronomy
- German
- Event Management
---
