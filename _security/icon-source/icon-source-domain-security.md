---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: iconsource.com
  spf: false
hosts:
- cert_expires: Oct 10 04:07:55 2026 GMT
  host: iconsource.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Icon Source Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Icon Source, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Icon Source
provider_slug: icon-source
slug: icon-source-domain-security
source_filename: icon-source-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: iconsource.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 04:07:55 2026 GMT\n  hsts: false\ndomains:\n- domain: iconsource.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/icon-source/refs/heads/main/security/icon-source-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Sports
- Athletes
- Marketing
- Advertising
- Influencer Marketing
- Marketplace
- NIL
- Sponsorship
- Higher Education
---
