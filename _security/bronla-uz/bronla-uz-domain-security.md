---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bronla.uz
  spf: true
hosts:
- host: bronla.uz
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bronla Uz Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for bronla-uz, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: bronla-uz
provider_slug: bronla-uz
slug: bronla-uz-domain-security
source_filename: bronla-uz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bronla.uz\n  https: false\ndomains:\n- domain: bronla.uz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/bronla-uz/security/bronla-uz-domain-security.yml
summary_line: DMARC
tags:
- Company
---
