---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: isdayoff.ru
  spf: false
hosts:
- cert_expires: Oct  1 12:27:59 2026 GMT
  host: isdayoff.ru
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Non Working Days Isdayoff Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Non-Working Days, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Non-Working Days
provider_slug: non-working-days-isdayoff
slug: non-working-days-isdayoff-domain-security
source_filename: non-working-days-isdayoff-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: isdayoff.ru\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 12:27:59 2026 GMT\n  hsts: false\ndomains:\n- domain: isdayoff.ru\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/non-working-days-isdayoff/refs/heads/main/security/non-working-days-isdayoff-domain-security.yml
summary_line: TLSv1.3
tags:
- Calendar
- Public APIs
---
