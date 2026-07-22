---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: kilo.vn
  spf: true
hosts:
- host: kilo.vn
  https: false
kind: domain-security
layout: security
method: probed
name: Kilo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kilo, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Kilo
provider_slug: kilo
slug: kilo-domain-security
source_filename: kilo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kilo.vn\n  https: false\ndomains:\n- domain: kilo.vn\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kilo/refs/heads/main/security/kilo-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
---
