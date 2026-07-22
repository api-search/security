---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lawnstarter.com
  spf: true
hosts:
- cert_expires: Sep 21 22:24:18 2026 GMT
  host: lawnstarter.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lawnstarter Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LawnStarter, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: LawnStarter
provider_slug: lawnstarter
slug: lawnstarter-domain-security
source_filename: lawnstarter-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lawnstarter.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 22:24:18 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: lawnstarter.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lawnstarter/refs/heads/main/security/lawnstarter-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Lawn Care
- Landscaping
- Home Services
- Marketplace
- On-Demand
- Local Services
---
