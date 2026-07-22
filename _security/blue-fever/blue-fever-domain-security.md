---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: bluefever.com
  spf: false
hosts:
- cert_expires: Oct  6 07:46:44 2026 GMT
  host: bluefever.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Blue Fever Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Blue Fever, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Blue Fever
provider_slug: blue-fever
slug: blue-fever-domain-security
source_filename: blue-fever-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bluefever.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 07:46:44 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: bluefever.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blue-fever/refs/heads/main/security/blue-fever-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Mental Health
- Social
- Wellness
- AI
- Consumer App
- Teens
- Emotional Support
---
