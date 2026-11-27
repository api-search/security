---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: appcircle.io
  spf: true
hosts:
- cert_expires: Jan 27 12:13:22 2027 GMT
  host: appcircle.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Appcircle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Appcircle, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Appcircle
provider_slug: appcircle-io
slug: appcircle-io-domain-security
source_filename: appcircle-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: appcircle.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 12:13:22 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: appcircle.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/appcircle-io/security/appcircle-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Mobile
- CI/CD
- Automation
- iOS
- Android
---
