---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fairline.io
  spf: true
hosts:
- cert_expires: Jan 11 12:14:00 2027 GMT
  host: fairline.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fairline Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fairline, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Fairline
provider_slug: fairline-io
slug: fairline-io-domain-security
source_filename: fairline-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fairline.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 12:14:00 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: fairline.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/fairline-io/security/fairline-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Sports Betting
- Analytics
- MLB
- NHL
- EPL
- NFL
---
