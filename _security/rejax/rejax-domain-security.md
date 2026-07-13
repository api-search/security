---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: rejax.io
  spf: true
hosts:
- host: rejax.io
  https: false
kind: domain-security
layout: security
method: probed
name: Rejax Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rejax, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Rejax
provider_slug: rejax
slug: rejax-domain-security
source_filename: rejax-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rejax.io\n  https: false\ndomains:\n- domain: rejax.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rejax/refs/heads/main/security/rejax-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Development
- Public APIs
---
