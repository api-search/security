---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: internationalcall.co
  spf: false
hosts:
- cert_expires: Feb  6 06:02:03 2027 GMT
  host: internationalcall.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: InternationalCall.co Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for InternationalCall.co, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: InternationalCall.co
provider_slug: internationalcall-co
slug: internationalcall-co-domain-security
source_filename: internationalcall-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: internationalcall.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  6 06:02:03 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: internationalcall.co\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/internationalcall-co/security/internationalcall-co-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Telephony
- VoIP
- BrowserApp
- InternationalCalls
- Software-as-a-Service
---
