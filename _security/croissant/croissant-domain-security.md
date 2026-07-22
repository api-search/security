---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: getcroissant.com
  spf: true
hosts:
- cert_expires: Oct 14 10:03:13 2026 GMT
  host: getcroissant.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Croissant Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Croissant, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Croissant
provider_slug: croissant
slug: croissant-domain-security
source_filename: croissant-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getcroissant.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 10:03:13 2026 GMT\n  hsts: false\ndomains:\n- domain: getcroissant.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/croissant/refs/heads/main/security/croissant-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Coworking
- Workspace Management
- Distributed Teams
- Real Estate
- Spend Management
- Booking
- SaaS
---
