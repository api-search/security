---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: mailhaven.co
  spf: true
hosts:
- host: mailhaven.co
  https: false
kind: domain-security
layout: security
method: probed
name: Mailhaven Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mailhaven, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Mailhaven
provider_slug: mailhaven
slug: mailhaven-domain-security
source_filename: mailhaven-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mailhaven.co\n  https: false\ndomains:\n- domain: mailhaven.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mailhaven/refs/heads/main/security/mailhaven-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
---
