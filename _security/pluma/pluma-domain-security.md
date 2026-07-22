---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: pluma.co
  spf: true
hosts:
- host: pluma.co
  https: false
kind: domain-security
layout: security
method: probed
name: Pluma Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pluma, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Pluma
provider_slug: pluma
slug: pluma-domain-security
source_filename: pluma-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pluma.co\n  https: false\ndomains:\n- domain: pluma.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pluma/refs/heads/main/security/pluma-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
---
