---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: trulyexperiences.com
  spf: true
hosts:
- cert_expires: Oct  4 15:44:38 2026 GMT
  host: trulyexperiences.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Truly Experiences Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Truly Experiences, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Truly Experiences
provider_slug: truly-experiences
slug: truly-experiences-domain-security
source_filename: truly-experiences-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: trulyexperiences.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 15:44:38 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: trulyexperiences.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/truly-experiences/refs/heads/main/security/truly-experiences-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Experiences
- Gifting
- Ecommerce
- Travel
- Hospitality
- Consumer
- United Kingdom
---
