---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kardome.com
  spf: true
hosts:
- cert_expires: Oct  4 18:07:23 2026 GMT
  host: kardome.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kardome Technology Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kardome Technology, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Kardome Technology
provider_slug: kardome-technology
slug: kardome-technology-domain-security
source_filename: kardome-technology-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kardome.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 18:07:23 2026 GMT\n  hsts: null\ndomains:\n- domain: kardome.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kardome-technology/refs/heads/main/security/kardome-technology-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Voice AI
- Speech Recognition
- Automotive
- Smart Home
- Audio
- Machine Learning
- Voice Interface
---
