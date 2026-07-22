---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wizzpass.com
  spf: true
hosts:
- host: wizzpass.com
  https: false
kind: domain-security
layout: security
method: probed
name: Wizzpass Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WizzPass, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: WizzPass
provider_slug: wizzpass
slug: wizzpass-domain-security
source_filename: wizzpass-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wizzpass.com\n  https: false\ndomains:\n- domain: wizzpass.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wizzpass/refs/heads/main/security/wizzpass-domain-security.yml
summary_line: DMARC
tags:
- Company
- Visitor Management
- Access Control
- Workplace
- Security
- Techstars
---
