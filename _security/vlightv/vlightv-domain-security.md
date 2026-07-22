---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: vlightv.com
  spf: true
hosts:
- host: vlightv.com
  https: false
kind: domain-security
layout: security
method: probed
name: Vlightv Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for vlightv, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: vlightv
provider_slug: vlightv
slug: vlightv-domain-security
source_filename: vlightv-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vlightv.com\n  https: false\ndomains:\n- domain: vlightv.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vlightv/refs/heads/main/security/vlightv-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
---
