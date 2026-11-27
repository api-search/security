---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: adsgpt.dev
  spf: true
hosts:
- cert_expires: Jan 12 17:07:42 2027 GMT
  host: adsgpt.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  6 12:02:10 2027 GMT
  host: docs.adsgpt.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: AdsGPT Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AdsGPT, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: AdsGPT
provider_slug: adsgpt-dev
slug: adsgpt-dev-domain-security
source_filename: adsgpt-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: adsgpt.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 17:07:42 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.adsgpt.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 12:02:10 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: adsgpt.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/adsgpt-dev/security/adsgpt-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Advertising
- Artificial Intelligence
- Marketing
- Automation
- Platform
---
