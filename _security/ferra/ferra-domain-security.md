---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ferra.club
  spf: false
hosts:
- cert_expires: Sep 30 00:32:10 2026 GMT
  host: ferra.club
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ferra Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ferra, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Ferra
provider_slug: ferra
slug: ferra-domain-security
source_filename: ferra-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ferra.club\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 00:32:10 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ferra.club\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ferra/refs/heads/main/security/ferra-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Fitness
- Health
- Wellness
- Strength Training
- Connected Hardware
- Subscription
- Aging
- India
---
