---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: figure1.com
  spf: true
hosts:
- cert_expires: Oct  3 10:31:14 2026 GMT
  host: figure1.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Figure1 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Figure1, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Figure1
provider_slug: figure1
slug: figure1-domain-security
source_filename: figure1-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: figure1.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 10:31:14 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: figure1.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/figure1/refs/heads/main/security/figure1-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Medical Education
- Health
- Social Network
- Mobile App
- Clinical
- Physicians
---
