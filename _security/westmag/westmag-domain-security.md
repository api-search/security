---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: westmag.com
  spf: false
hosts:
- cert_expires: Aug 27 15:27:04 2026 GMT
  host: www.westmag.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Westmag Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Westmag, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Westmag
provider_slug: westmag
slug: westmag-domain-security
source_filename: westmag-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.westmag.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 15:27:04 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: westmag.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/westmag/refs/heads/main/security/westmag-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Hardware
- Robotics
- Drones
- Motors
- Actuators
- Manufacturing
- BLDC
- Defense
---
