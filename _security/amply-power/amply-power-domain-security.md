---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: amplypower.com
  spf: true
hosts:
- host: amplypower.com
  https: false
kind: domain-security
layout: security
method: probed
name: Amply Power Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amply Power, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Amply Power
provider_slug: amply-power
slug: amply-power-domain-security
source_filename: amply-power-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: amplypower.com\n  https: false\ndomains:\n- domain: amplypower.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amply-power/refs/heads/main/security/amply-power-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
---
