---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: abcfintech.com
  spf: true
hosts:
- host: abcfintech.com
  https: false
kind: domain-security
layout: security
method: probed
name: Abcfintech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for abcfintech, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: abcfintech
provider_slug: abcfintech
slug: abcfintech-domain-security
source_filename: abcfintech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: abcfintech.com\n  https: false\ndomains:\n- domain: abcfintech.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/abcfintech/refs/heads/main/security/abcfintech-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Fintech
- Financial Services
- Venture Backed
---
