---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sampler.io
  spf: true
hosts:
- host: sampler.io
  https: false
kind: domain-security
layout: security
method: probed
name: Sampler Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sampler, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sampler
provider_slug: sampler
slug: sampler-domain-security
source_filename: sampler-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sampler.io\n  https: false\ndomains:\n- domain: sampler.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sampler/refs/heads/main/security/sampler-domain-security.yml
summary_line: DMARC
tags:
- Company
- Marketing
- Product Sampling
- Consumer Packaged Goods
- Advertising
- SaaS
---
