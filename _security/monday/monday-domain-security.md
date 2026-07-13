---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: monday.com
  spf: true
hosts:
- host: api.developer.monday.com
  https: false
kind: domain-security
layout: security
method: probed
name: Monday Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Monday, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Monday
provider_slug: monday
slug: monday-domain-security
source_filename: monday-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.developer.monday.com\n  https: false\ndomains:\n- domain: monday.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/monday/refs/heads/main/security/monday-domain-security.yml
summary_line: DMARC
tags:
- Documents And Productivity
- Public APIs
---
