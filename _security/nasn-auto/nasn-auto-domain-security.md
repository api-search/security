---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nasn-auto.com
  spf: true
hosts:
- host: nasn-auto.com
  https: false
kind: domain-security
layout: security
method: probed
name: Nasn Auto Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for nasn-auto, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: nasn-auto
provider_slug: nasn-auto
slug: nasn-auto-domain-security
source_filename: nasn-auto-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nasn-auto.com\n  https: false\ndomains:\n- domain: nasn-auto.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nasn-auto/refs/heads/main/security/nasn-auto-domain-security.yml
summary_line: DMARC
tags:
- Company
- Automotive
- Automotive Electronics
- Brake-by-Wire
- Steer-by-Wire
- Autonomous Driving
- Hardware
- Manufacturing
- China
---
