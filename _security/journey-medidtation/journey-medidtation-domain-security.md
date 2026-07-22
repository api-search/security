---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: journey.live
  spf: true
hosts:
- cert_expires: Aug 27 10:39:56 2026 GMT
  host: journey.live
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Journey Medidtation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Journey Medidtation, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Journey Medidtation
provider_slug: journey-medidtation
slug: journey-medidtation-domain-security
source_filename: journey-medidtation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: journey.live\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 10:39:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: journey.live\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/journey-medidtation/refs/heads/main/security/journey-medidtation-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Mental Health
- Employee Assistance Program
- Wellbeing
- Meditation
- Healthcare
- HR Technology
- Enterprise
---
