---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: prana.health
  spf: false
hosts:
- cert_expires: Oct 11 06:29:36 2026 GMT
  host: prana.health
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Prana Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Prana Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Prana Health
provider_slug: prana-health
slug: prana-health-domain-security
source_filename: prana-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: prana.health\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 06:29:36 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: prana.health\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prana-health/refs/heads/main/security/prana-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Health
- Fitness
- Longevity
- Body Composition
- Personalized Medicine
- Consumer Health
- Machine Learning
---
