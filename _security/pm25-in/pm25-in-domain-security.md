---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: pm25.in
  spf: true
hosts:
- host: www.pm25.in
  https: false
kind: domain-security
layout: security
method: probed
name: Pm25 In Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PM25.in, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: PM25.in
provider_slug: pm25-in
slug: pm25-in-domain-security
source_filename: pm25-in-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pm25.in\n  https: false\ndomains:\n- domain: pm25.in\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pm25-in/refs/heads/main/security/pm25-in-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Environment
- Public APIs
---
