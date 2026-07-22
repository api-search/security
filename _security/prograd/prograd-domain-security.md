---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: prograd.uk
  spf: true
hosts:
- cert_expires: Sep 18 20:21:42 2026 GMT
  host: prograd.uk
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Prograd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ProGrad, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ProGrad
provider_slug: prograd
slug: prograd-domain-security
source_filename: prograd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: prograd.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 20:21:42 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: prograd.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prograd/refs/heads/main/security/prograd-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Rewards
- Mobile App
- Fintech
- Gen Z
- United Kingdom
---
