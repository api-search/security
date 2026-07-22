---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: usermind.com
  spf: true
hosts:
- host: usermind.com
  https: false
kind: domain-security
layout: security
method: probed
name: Usermind Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Usermind, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Usermind
provider_slug: usermind
slug: usermind-domain-security
source_filename: usermind-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: usermind.com\n  https: false\ndomains:\n- domain: usermind.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/usermind/refs/heads/main/security/usermind-domain-security.yml
summary_line: DMARC
tags:
- Company
- Customer Journey
- Journey Orchestration
- Customer Experience
- Marketing Technology
- Acquired
---
