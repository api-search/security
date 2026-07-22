---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: winglang.io
  spf: true
hosts:
- host: www.winglang.io
  https: false
kind: domain-security
layout: security
method: probed
name: Wing Cloud Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wing Cloud, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Wing Cloud
provider_slug: wing-cloud
slug: wing-cloud-domain-security
source_filename: wing-cloud-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.winglang.io\n  https: false\ndomains:\n- domain: winglang.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wing-cloud/refs/heads/main/security/wing-cloud-domain-security.yml
summary_line: DMARC
tags:
- Company
- Programming Language
- Cloud Development
- Infrastructure as Code
- Developer Tools
- Open Source
- SDK
- CLI
---
