---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tonal.com
  spf: true
hosts:
- cert_expires: Sep  9 02:07:33 2026 GMT
  host: tonal.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tonal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tonal, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Tonal
provider_slug: tonal
slug: tonal-domain-security
source_filename: tonal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tonal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 02:07:33 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: tonal.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tonal/refs/heads/main/security/tonal-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Health Wellness
- Fitness
- Strength Training
- Connected Fitness
- Home Gym
- Coaching
- Wellness
---
