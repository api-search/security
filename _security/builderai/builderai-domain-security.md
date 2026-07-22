---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: builder.ai
  spf: true
hosts:
- host: www.builder.ai
  https: false
kind: domain-security
layout: security
method: probed
name: Builderai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Builder.ai, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Builder.ai
provider_slug: builderai
slug: builderai-domain-security
source_filename: builderai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.builder.ai\n  https: false\ndomains:\n- domain: builder.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/builderai/refs/heads/main/security/builderai-domain-security.yml
summary_line: DMARC
tags:
- Company
- Artificial Intelligence
- Application Development
- No Code
- Low Code
- App Builder
- Software Development
- Defunct
---
