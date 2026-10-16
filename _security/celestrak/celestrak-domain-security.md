---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: celestrak.org
  spf: false
hosts:
- host: celestrak.org
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Celestrak Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CelesTrak, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: CelesTrak
provider_slug: celestrak
slug: celestrak-domain-security
source_filename: celestrak-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: celestrak.org\n  https: false\ndomains:\n- domain: celestrak.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/celestrak/refs/heads/main/security/celestrak-domain-security.yml
summary_line: DMARC
tags:
- Company
---
