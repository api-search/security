---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mela.work
  spf: true
hosts:
- cert_expires: Sep 19 23:59:59 2026 GMT
  host: mela.work
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Mela Works Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mela Works, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Mela Works
provider_slug: mela-works
slug: mela-works-domain-security
source_filename: mela-works-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mela.work\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 19 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: mela.work\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mela-works/refs/heads/main/security/mela-works-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Construction
- Construction Tech
- Field Service
- Site Management
- Project Management
- Productivity
- Mobile
- AI
- Document Management
- SaaS
---
