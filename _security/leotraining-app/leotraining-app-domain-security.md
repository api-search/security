---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: leotraining.app
  spf: true
hosts:
- cert_expires: Dec 18 09:47:40 2026 GMT
  host: leotraining.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Leo Training Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Leo Training, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Leo Training
provider_slug: leotraining-app
slug: leotraining-app-domain-security
source_filename: leotraining-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: leotraining.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 09:47:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: leotraining.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/leotraining-app/security/leotraining-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Coaching
- Running
- Cycling
- Triathlon
- Subscription
---
