---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: eversightlabs.com
  spf: true
hosts:
- host: eversightlabs.com
  https: false
kind: domain-security
layout: security
method: probed
name: Eversight Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Eversight, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Eversight
provider_slug: eversight
slug: eversight-domain-security
source_filename: eversight-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: eversightlabs.com\n  https: false\ndomains:\n- domain: eversightlabs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eversight/refs/heads/main/security/eversight-domain-security.yml
summary_line: DMARC
tags:
- Company
- Retail Tech
- Pricing
- Promotions
- CPG
- Artificial Intelligence
- Revenue Management
- SaaS
---
