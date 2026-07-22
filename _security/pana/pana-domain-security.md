---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: pana.com
  spf: true
hosts:
- host: pana.com
  https: false
kind: domain-security
layout: security
method: probed
name: Pana Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pana, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Pana
provider_slug: pana
slug: pana-domain-security
source_filename: pana-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pana.com\n  https: false\ndomains:\n- domain: pana.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pana/refs/heads/main/security/pana-domain-security.yml
summary_line: DMARC
tags:
- Company
---
