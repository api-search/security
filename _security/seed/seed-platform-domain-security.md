---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cantaloupe.com
  spf: true
hosts:
- host: api.cantaloupe.com
  https: false
kind: domain-security
layout: security
method: probed
name: Seed Platform Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Seed, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Seed
provider_slug: seed
slug: seed-platform-domain-security
source_filename: seed-platform-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.cantaloupe.com\n  https: false\ndomains:\n- domain: cantaloupe.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/seed/refs/heads/main/security/seed-platform-domain-security.yml
summary_line: DMARC
tags:
- Payments
- Sales
---
