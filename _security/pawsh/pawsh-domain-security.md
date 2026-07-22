---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: pawsh.app
  spf: true
hosts:
- cert_expires: Oct  6 06:39:24 2026 GMT
  host: pawsh.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pawsh Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pawsh, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Pawsh
provider_slug: pawsh
slug: pawsh-domain-security
source_filename: pawsh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pawsh.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 06:39:24 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: pawsh.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pawsh/refs/heads/main/security/pawsh-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Pet Care
- Grooming
- Marketplace
- Booking
- Pets
- Consumer
- Local Services
---
