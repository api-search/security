---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: oneswoop.com
  spf: true
hosts:
- host: www.oneswoop.com
  https: false
kind: domain-security
layout: security
method: probed
name: Oneswoop Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OneSwoop, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: OneSwoop
provider_slug: oneswoop
slug: oneswoop-domain-security
source_filename: oneswoop-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.oneswoop.com\n  https: false\ndomains:\n- domain: oneswoop.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oneswoop/refs/heads/main/security/oneswoop-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Automotive
- Cars
- Price Comparison
- E-Commerce
- United Kingdom
---
