---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: vonjour.com
  spf: true
hosts:
- host: vonjour.com
  https: false
kind: domain-security
layout: security
method: probed
name: Vonbox Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VonBox, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: VonBox
provider_slug: vonbox
slug: vonbox-domain-security
source_filename: vonbox-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vonjour.com\n  https: false\ndomains:\n- domain: vonjour.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vonbox/refs/heads/main/security/vonbox-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Communications
- Telephony
- Messaging
- Contact Centers
- Startups
---
