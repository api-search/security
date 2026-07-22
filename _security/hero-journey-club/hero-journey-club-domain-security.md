---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: herojourney.club
  spf: true
hosts:
- host: www.herojourney.club
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has expired (_ssl.c:1082)'
kind: domain-security
layout: security
method: probed
name: Hero Journey Club Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hero Journey Club, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Hero Journey Club
provider_slug: hero-journey-club
slug: hero-journey-club-domain-security
source_filename: hero-journey-club-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.herojourney.club\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has\n    expired (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: herojourney.club\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hero-journey-club/refs/heads/main/security/hero-journey-club-domain-security.yml
summary_line: DNSSEC · DMARC
tags:
- Company
- Healthcare
- Mental Health
- Wellness
- Digital Health
---
