---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: aosong.com
  spf: true
hosts:
- host: aosong.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aosongelectronics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aosongelectronics, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Aosongelectronics
provider_slug: aosongelectronics
slug: aosongelectronics-domain-security
source_filename: aosongelectronics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aosong.com\n  https: false\ndomains:\n- domain: aosong.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aosongelectronics/refs/heads/main/security/aosongelectronics-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Technology
- Electronics
- Manufacturing
- IoT
---
