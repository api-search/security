---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: buela.ai
  spf: true
hosts:
- host: buela.ai
  https: false
kind: domain-security
layout: security
method: probed
name: Buela Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Buela, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Buela
provider_slug: buela
slug: buela-domain-security
source_filename: buela-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: buela.ai\n  https: false\ndomains:\n- domain: buela.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/buela/refs/heads/main/security/buela-domain-security.yml
summary_line: DNSSEC · DMARC
tags:
- Company
---
