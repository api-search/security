---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ztock.app
  spf: true
hosts:
- host: ztock.app
  https: false
kind: domain-security
layout: security
method: probed
name: Ztock Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ztock, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Ztock
provider_slug: ztock
slug: ztock-domain-security
source_filename: ztock-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ztock.app\n  https: false\ndomains:\n- domain: ztock.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ztock/refs/heads/main/security/ztock-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
---
