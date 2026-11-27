---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mediawork.io
  spf: false
hosts:
- cert_expires: Feb  8 07:00:10 2027 GMT
  host: mediawork.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mediawork Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mediawork, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: Mediawork
provider_slug: mediawork-io
slug: mediawork-io-domain-security
source_filename: mediawork-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mediawork.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  8 07:00:10 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: mediawork.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/mediawork-io/security/mediawork-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- CRM
- Quoting
- Scheduling
- Cost Tracking
- Billing
- Media Production Management
- Post‑Production
- Freelance Creatives
---
