---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: coretechmed.com
  spf: true
hosts:
- host: coretechmed.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Coremedicaltechnology Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Coremedicaltechnology, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Coremedicaltechnology
provider_slug: coremedicaltechnology
slug: coremedicaltechnology-domain-security
source_filename: coremedicaltechnology-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: coretechmed.com\n  https: false\ndomains:\n- domain: coretechmed.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coremedicaltechnology/refs/heads/main/security/coremedicaltechnology-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Medical
- Devices
- ArtificialHeart
- China
- Healthcare
---
