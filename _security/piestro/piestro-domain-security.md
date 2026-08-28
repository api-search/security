---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: piestro.com
  spf: false
hosts:
- cert_expires: Oct 11 09:01:58 2026 GMT
  host: piestro.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Piestro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Piestro, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Piestro
provider_slug: piestro
slug: piestro-domain-security
source_filename: piestro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: piestro.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 09:01:58 2026 GMT\n  hsts: null\ndomains:\n- domain: piestro.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/piestro/refs/heads/main/security/piestro-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Robotics
- Automation
- Food Service
- Restaurant Technology
- Vending
- Hardware
- Defunct
---
