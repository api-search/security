---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: quickmocker.com
  spf: true
hosts:
- host: quickmocker.com
  https: false
kind: domain-security
layout: security
method: probed
name: Quickmocker Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for QuickMocker, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: QuickMocker
provider_slug: quickmocker
slug: quickmocker-domain-security
source_filename: quickmocker-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: quickmocker.com\n  https: false\ndomains:\n- domain: quickmocker.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quickmocker/refs/heads/main/security/quickmocker-domain-security.yml
summary_line: DMARC
tags:
- Test Data
- Public APIs
---
