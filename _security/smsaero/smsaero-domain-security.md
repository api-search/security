---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: smsaero.ru
  spf: true
hosts:
- cert_expires: Dec 20 13:04:57 2026 GMT
  host: smsaero.ru
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Smsaero Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SMS Aero, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: SMS Aero
provider_slug: smsaero
slug: smsaero-domain-security
source_filename: smsaero-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: smsaero.ru\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 20 13:04:57 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: smsaero.ru\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/smsaero/security/smsaero-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- SMS
- Messaging
- Bulk
- API
---
