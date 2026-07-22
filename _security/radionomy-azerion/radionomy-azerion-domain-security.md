---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  dmarc: false
  dnssec: false
  domain: radionomy.com
  spf: true
hosts:
- host: www.radionomy.com
  https: false
kind: domain-security
layout: security
method: probed
name: Radionomy Azerion Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Radionomy (Azerion), probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Radionomy (Azerion)
provider_slug: radionomy-azerion
slug: radionomy-azerion-domain-security
source_filename: radionomy-azerion-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.radionomy.com\n  https: false\ndomains:\n- domain: radionomy.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/radionomy-azerion/refs/heads/main/security/radionomy-azerion-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Ai Apps
- Audio
- Internet Radio
- Streaming
- Media
---
