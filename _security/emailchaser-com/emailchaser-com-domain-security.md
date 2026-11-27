---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: emailchaser.com
  spf: true
hosts:
- cert_expires: Jan  5 06:13:03 2027 GMT
  host: emailchaser.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Emailchaser Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Emailchaser, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Emailchaser
provider_slug: emailchaser-com
slug: emailchaser-com-domain-security
source_filename: emailchaser-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: emailchaser.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 06:13:03 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: emailchaser.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/emailchaser-com/security/emailchaser-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cold Email
- Sales
- Marketing
- Lead Generation
- Software-as-a-Service
---
