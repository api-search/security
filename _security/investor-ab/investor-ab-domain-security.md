---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: investorab.com
  spf: true
hosts:
- host: investorab.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Investor Ab Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Investor AB, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Investor AB
provider_slug: investor-ab
slug: investor-ab-domain-security
source_filename: investor-ab-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: investorab.com\n  https: false\ndomains:\n- domain: investorab.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/investor-ab/refs/heads/main/security/investor-ab-domain-security.yml
summary_line: DMARC
tags:
- Company
---
