---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gymnadz.com
  spf: true
hosts:
- cert_expires: Sep  8 06:38:09 2026 GMT
  host: gymnadz.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gymnadz Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GymNadz, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: GymNadz
provider_slug: gymnadz
slug: gymnadz-domain-security
source_filename: gymnadz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gymnadz.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 06:38:09 2026 GMT\n  hsts: false\ndomains:\n- domain: gymnadz.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gymnadz/refs/heads/main/security/gymnadz-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Fitness
- Health
- Wellness
- Mobile
- Nutrition
- Women
- Consumer App
---
