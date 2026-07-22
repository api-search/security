---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: benrevo.com
  spf: true
hosts:
- host: benrevo.com
  https: false
kind: domain-security
layout: security
method: probed
name: Benrevo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BenRevo, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: BenRevo
provider_slug: benrevo
slug: benrevo-domain-security
source_filename: benrevo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: benrevo.com\n  https: false\ndomains:\n- domain: benrevo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/benrevo/refs/heads/main/security/benrevo-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
---
