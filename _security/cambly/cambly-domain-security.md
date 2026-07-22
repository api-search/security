---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cambly.com
  spf: true
hosts:
- cert_expires: Aug 26 21:43:51 2026 GMT
  host: www.cambly.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cambly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cambly, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cambly
provider_slug: cambly
slug: cambly-domain-security
source_filename: cambly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cambly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 21:43:51 2026 GMT\n  hsts: false\ndomains:\n- domain: cambly.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cambly/refs/heads/main/security/cambly-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Consumer
- Education
- Language Learning
- EdTech
- Tutoring
- Video
- Marketplace
---
