---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: fitcolatam.com
  spf: true
hosts:
- cert_expires: Aug 31 20:19:07 2026 GMT
  host: fitcolatam.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fitco Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FITCO, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: FITCO
provider_slug: fitco
slug: fitco-domain-security
source_filename: fitco-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fitcolatam.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 20:19:07 2026 GMT\n  hsts: false\ndomains:\n- domain: fitcolatam.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fitco/refs/heads/main/security/fitco-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Fitness
- Gym Management
- SaaS
- Latin America
- Bookings
- Memberships
- Payments
- Wellness
- Boutique Fitness
---
