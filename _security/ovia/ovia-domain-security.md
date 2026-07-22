---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: wepow.com
  spf: true
hosts:
- cert_expires: Oct 17 00:49:58 2026 GMT
  host: wepow.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ovia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OVIA, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: OVIA
provider_slug: ovia
slug: ovia-domain-security
source_filename: ovia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wepow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 00:49:58 2026 GMT\n  hsts: false\ndomains:\n- domain: wepow.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ovia/refs/heads/main/security/ovia-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Recruiting
- Talent Assessment
- Video Interviewing
- Human Resources
- Hiring
- HR Tech
---
