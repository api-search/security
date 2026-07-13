---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: saidit.net
  spf: true
hosts:
- host: www.saidit.net
  https: false
kind: domain-security
layout: security
method: probed
name: Saidit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Saidit, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Saidit
provider_slug: saidit
slug: saidit-domain-security
source_filename: saidit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.saidit.net\n  https: false\ndomains:\n- domain: saidit.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/saidit/refs/heads/main/security/saidit-domain-security.yml
summary_line: DMARC
tags:
- Social
- Public APIs
---
