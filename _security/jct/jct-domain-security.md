---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: jct.com
  spf: true
hosts:
- host: jct.com
  https: false
kind: domain-security
layout: security
method: probed
name: Jct Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for jct, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: jct
provider_slug: jct
slug: jct-domain-security
source_filename: jct-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jct.com\n  https: false\ndomains:\n- domain: jct.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jct/refs/heads/main/security/jct-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
---
