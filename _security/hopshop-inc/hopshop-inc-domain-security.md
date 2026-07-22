---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hopshop.ai
  spf: true
hosts:
- host: hopshop.ai
  https: false
kind: domain-security
layout: security
method: probed
name: Hopshop Inc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HopShop Inc., probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: HopShop Inc.
provider_slug: hopshop-inc
slug: hopshop-inc-domain-security
source_filename: hopshop-inc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hopshop.ai\n  https: false\ndomains:\n- domain: hopshop.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hopshop-inc/refs/heads/main/security/hopshop-inc-domain-security.yml
summary_line: DMARC
tags:
- Company
- Fashion
- Retail
- E-Commerce
- Visual Search
- Artificial Intelligence
- Creator Economy
- Shopping
---
