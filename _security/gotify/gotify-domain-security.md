---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: gotify.net
  spf: true
hosts:
- cert_expires: Jan 17 13:35:20 2027 GMT
  host: gotify.net
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Gotify Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gotify, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Gotify
provider_slug: gotify
slug: gotify-domain-security
source_filename: gotify-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gotify.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 13:35:20 2027 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: gotify.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/gotify/security/gotify-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Messaging
- OpenSource
- SelfHosted
- Notifications
- API
---
