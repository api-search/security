---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: sendbloom.com
  spf: true
hosts:
- host: sendbloom.com
  https: false
kind: domain-security
layout: security
method: probed
name: Sendbloom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for sendbloom, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: sendbloom
provider_slug: sendbloom
slug: sendbloom-domain-security
source_filename: sendbloom-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sendbloom.com\n  https: false\ndomains:\n- domain: sendbloom.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sendbloom/refs/heads/main/security/sendbloom-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
---
