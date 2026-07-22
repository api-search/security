---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: tastespace.co
  spf: true
hosts:
- host: tastespace.co
  https: false
kind: domain-security
layout: security
method: probed
name: Semeantoja Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Semeantoja, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Semeantoja
provider_slug: semeantoja
slug: semeantoja-domain-security
source_filename: semeantoja-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tastespace.co\n  https: false\ndomains:\n- domain: tastespace.co\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/semeantoja/refs/heads/main/security/semeantoja-domain-security.yml
summary_line: DNSSEC
tags:
- Company
---
