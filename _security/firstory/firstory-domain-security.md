---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: firstory.me
  spf: true
hosts:
- cert_expires: Sep 24 23:59:59 2026 GMT
  host: firstory.me
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Firstory Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Firstory, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Firstory
provider_slug: firstory
slug: firstory-domain-security
source_filename: firstory-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: firstory.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: firstory.me\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/firstory/refs/heads/main/security/firstory-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Podcasting
- Podcast Hosting
- Media
- Audio
- Monetization
- Analytics
- Creator Tools
- Asia-Pacific
---
