---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: redcarpetup.com
  spf: true
hosts:
- host: redcarpetup.com
  https: false
kind: domain-security
layout: security
method: probed
name: Redcarpetup Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Redcarpetup, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Redcarpetup
provider_slug: redcarpetup
slug: redcarpetup-domain-security
source_filename: redcarpetup-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: redcarpetup.com\n  https: false\ndomains:\n- domain: redcarpetup.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/redcarpetup/refs/heads/main/security/redcarpetup-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Fintech
- Lending
- Consumer Credit
- India
---
