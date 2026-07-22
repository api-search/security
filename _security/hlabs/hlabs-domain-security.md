---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: hlaboratories.com
  spf: false
hosts:
- cert_expires: Sep 20 05:42:38 2026 GMT
  host: www.hlaboratories.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hlabs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hlabs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Hlabs
provider_slug: hlabs
slug: hlabs-domain-security
source_filename: hlabs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hlaboratories.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 05:42:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hlaboratories.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hlabs/refs/heads/main/security/hlabs-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Robotics
- Hardware
- Robots
- Electronics
- Actuators
- Motors
- Manufacturing
- Y Combinator
---
