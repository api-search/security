---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: open.store
  spf: true
hosts:
- host: open.store
  https: false
kind: domain-security
layout: security
method: probed
name: Openstore Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenStore, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: OpenStore
provider_slug: openstore
slug: openstore-domain-security
source_filename: openstore-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: open.store\n  https: false\ndomains:\n- domain: open.store\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openstore/refs/heads/main/security/openstore-domain-security.yml
summary_line: DMARC
tags:
- Company
- E-Commerce
- Shopify
- Direct-to-Consumer
- Acquisitions
- Retail
- Holding Company
---
