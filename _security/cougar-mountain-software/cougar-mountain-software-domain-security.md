---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cougarmtn.com
  spf: true
hosts:
- cert_expires: Dec 14 08:48:03 2026 GMT
  host: cougarmtn.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cougar Mountain Software Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cougar Mountain Software, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cougar Mountain Software
provider_slug: cougar-mountain-software
slug: cougar-mountain-software-domain-security
source_filename: cougar-mountain-software-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cougarmtn.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 08:48:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cougarmtn.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/cougar-mountain-software/security/cougar-mountain-software-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Accounting
- Software
- Nonprofit
- Small Business
- Government
- On-Premise
---
