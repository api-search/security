---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: eigencomm.com
  spf: true
hosts:
- host: eigencomm.com
  https: false
kind: domain-security
layout: security
method: probed
name: Eigencomm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for eigencomm, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: eigencomm
provider_slug: eigencomm
slug: eigencomm-domain-security
source_filename: eigencomm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: eigencomm.com\n  https: false\ndomains:\n- domain: eigencomm.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eigencomm/refs/heads/main/security/eigencomm-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Semiconductor
- Chipsets
- Internet of Things
- Cellular IoT
- NB-IoT
- 5G
- Hardware
---
