---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: boostorder.com
  spf: true
hosts:
- host: boostorder.com
  https: false
kind: domain-security
layout: security
method: probed
name: Instanture Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Instanture, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Instanture
provider_slug: instanture
slug: instanture-domain-security
source_filename: instanture-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: boostorder.com\n  https: false\ndomains:\n- domain: boostorder.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/instanture/refs/heads/main/security/instanture-domain-security.yml
summary_line: DMARC
tags:
- Company
---
