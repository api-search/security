---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: tingsn.com
  spf: true
hosts:
- host: tingsn.com
  https: false
kind: domain-security
layout: security
method: probed
name: Tingsn Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tingsn, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Tingsn
provider_slug: tingsn
slug: tingsn-domain-security
source_filename: tingsn-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tingsn.com\n  https: false\ndomains:\n- domain: tingsn.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tingsn/refs/heads/main/security/tingsn-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Medical Devices
- Healthcare
- Cardiology
- Ultrasound
- Imaging
---
