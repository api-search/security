---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: abalin.net
  spf: true
hosts:
- cert_expires: Aug 21 14:16:20 2026 GMT
  host: nameday.abalin.net
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Namedays Calendar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Namedays Calendar, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Namedays Calendar
provider_slug: namedays-calendar
slug: namedays-calendar-domain-security
source_filename: namedays-calendar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nameday.abalin.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 14:16:20 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: abalin.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/namedays-calendar/refs/heads/main/security/namedays-calendar-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Calendar
- Public APIs
---
