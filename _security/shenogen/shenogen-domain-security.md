---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: shenogen.com
  spf: true
hosts:
- host: shenogen.com
  https: false
kind: domain-security
layout: security
method: probed
name: Shenogen Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for shenogen, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: shenogen
provider_slug: shenogen
slug: shenogen-domain-security
source_filename: shenogen-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: shenogen.com\n  https: false\ndomains:\n- domain: shenogen.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shenogen/refs/heads/main/security/shenogen-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
---
