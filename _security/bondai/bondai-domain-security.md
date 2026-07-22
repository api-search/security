---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: bondai.io
  spf: false
hosts:
- cert_expires: Sep 21 05:26:42 2026 GMT
  host: bondai.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bondai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bondai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Bondai
provider_slug: bondai
slug: bondai-domain-security
source_filename: bondai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bondai.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 05:26:42 2026 GMT\n  hsts: false\ndomains:\n- domain: bondai.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bondai/refs/heads/main/security/bondai-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Travel
- Trip Planning
- Group Travel
- Experiences
- Booking
- Mobile App
- Tourism
---
