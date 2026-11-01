---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ctrl-therapeutics.com
  spf: true
hosts:
- host: www.ctrl-therapeutics.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ctrl Therapeutics Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ctrl Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Ctrl Therapeutics
provider_slug: ctrl-therapeutics-com
slug: ctrl-therapeutics-com-domain-security
source_filename: ctrl-therapeutics-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ctrl-therapeutics.com\n  https: false\ndomains:\n- domain: ctrl-therapeutics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/ctrl-therapeutics-com/security/ctrl-therapeutics-com-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
---
