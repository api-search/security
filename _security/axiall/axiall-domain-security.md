---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: axiall.com
  spf: true
hosts:
- host: www.axiall.com
  https: false
kind: domain-security
layout: security
method: probed
name: Axiall Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Axiall, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Axiall
provider_slug: axiall
slug: axiall-domain-security
source_filename: axiall-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.axiall.com\n  https: false\ndomains:\n- domain: axiall.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/axiall/refs/heads/main/security/axiall-domain-security.yml
summary_line: DMARC
tags:
- Chemicals
- Manufacturing
- Building Products
---
