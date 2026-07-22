---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: seculert.com
  spf: true
hosts:
- host: seculert.com
  https: false
kind: domain-security
layout: security
method: probed
name: Seculert Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Seculert, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Seculert
provider_slug: seculert
slug: seculert-domain-security
source_filename: seculert-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: seculert.com\n  https: false\ndomains:\n- domain: seculert.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/seculert/refs/heads/main/security/seculert-domain-security.yml
summary_line: DMARC
tags:
- Company
- Cybersecurity
- Threat Detection
- Security
- Analytics
- Acquired
- Defunct
---
