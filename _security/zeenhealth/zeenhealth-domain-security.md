---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: zeenhealth.com
  spf: true
hosts:
- host: zeenhealth.com
  https: false
kind: domain-security
layout: security
method: probed
name: Zeenhealth Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for zeenhealth, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: zeenhealth
provider_slug: zeenhealth
slug: zeenhealth-domain-security
source_filename: zeenhealth-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zeenhealth.com\n  https: false\ndomains:\n- domain: zeenhealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zeenhealth/refs/heads/main/security/zeenhealth-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Healthcare
- Health
- Digital Health
- China
---
