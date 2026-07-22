---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: zchb-water.net
  spf: true
hosts:
- host: zchb-water.net
  https: false
kind: domain-security
layout: security
method: probed
name: Zchb Water Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for zchb-water, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: zchb-water
provider_slug: zchb-water
slug: zchb-water-domain-security
source_filename: zchb-water-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zchb-water.net\n  https: false\ndomains:\n- domain: zchb-water.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zchb-water/refs/heads/main/security/zchb-water-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
---
