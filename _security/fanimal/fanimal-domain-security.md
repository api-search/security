---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: fanimal.com
  spf: true
hosts:
- cert_expires: Sep 22 06:19:13 2026 GMT
  host: fanimal.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fanimal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fanimal, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Fanimal
provider_slug: fanimal
slug: fanimal-domain-security
source_filename: fanimal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fanimal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 06:19:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fanimal.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fanimal/refs/heads/main/security/fanimal-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Defunct
- Events
- Ticketing
- Marketplace
---
