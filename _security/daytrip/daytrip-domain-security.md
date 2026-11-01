---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: daytrip.com
  spf: true
hosts:
- cert_expires: May  2 23:59:59 2027 GMT
  host: daytrip.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Daytrip Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Daytrip, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Daytrip
provider_slug: daytrip
slug: daytrip-domain-security
source_filename: daytrip-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: daytrip.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: May  2 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: daytrip.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/daytrip/security/daytrip-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Travel
- Transportation
- Booking
- Platform
---
