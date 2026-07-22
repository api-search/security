---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: jadend.tech
  spf: true
hosts:
- cert_expires: Sep 17 14:45:37 2026 GMT
  host: www.jadend.tech
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jade Autism Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jade Autism, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Jade Autism
provider_slug: jade-autism
slug: jade-autism-domain-security
source_filename: jade-autism-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.jadend.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 14:45:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: jadend.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jade-autism/refs/heads/main/security/jade-autism-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Education
- EdTech
- Autism
- Neurodiversity
- Accessibility
- Healthcare
- Mobile
- Eye Tracking
---
