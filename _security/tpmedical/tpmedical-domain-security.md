---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: tpmedical.com
  spf: true
hosts:
- host: tpmedical.com
  https: false
kind: domain-security
layout: security
method: probed
name: Tpmedical Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SMTP Technology, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: SMTP Technology
provider_slug: tpmedical
slug: tpmedical-domain-security
source_filename: tpmedical-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tpmedical.com\n  https: false\ndomains:\n- domain: tpmedical.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tpmedical/refs/heads/main/security/tpmedical-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Medical Devices
- Healthcare
- Surgical Equipment
- Ultrasonic Surgery
- Orthopedics
- Neurosurgery
---
