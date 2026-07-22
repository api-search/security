---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: alcatel-lucent.com
  spf: true
hosts:
- host: alcatel-lucent.com
  https: false
kind: domain-security
layout: security
method: probed
name: Alcatel Lucent Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alcatel-lucent, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Alcatel-lucent
provider_slug: alcatel-lucent
slug: alcatel-lucent-domain-security
source_filename: alcatel-lucent-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: alcatel-lucent.com\n  https: false\ndomains:\n- domain: alcatel-lucent.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alcatel-lucent/refs/heads/main/security/alcatel-lucent-domain-security.yml
summary_line: DMARC
tags:
- Company
- Telecommunications
- Networking
- Telecom Equipment
- Broadband
- Optical Networking
- Nokia
- Bell Labs
---
