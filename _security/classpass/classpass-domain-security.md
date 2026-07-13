---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: classpass.com
  spf: true
hosts:
- cert_expires: Sep 29 03:13:58 2026 GMT
  host: classpass.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 14 03:30:45 2026 GMT
  host: developers.classpass.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Classpass Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ClassPass, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ClassPass
provider_slug: classpass
slug: classpass-domain-security
source_filename: classpass-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: classpass.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 03:13:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.classpass.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 03:30:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: classpass.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/classpass/refs/heads/main/security/classpass-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fitness
- Wellness
- Class Booking
- Marketplace
- Studios
- Gyms
- Scheduling
- Partner API
---
