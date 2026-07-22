---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: fancy.tech
  spf: true
hosts:
- host: www.fancy.tech
  https: false
kind: domain-security
layout: security
method: probed
name: Fancy Technology Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fancy Technology, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Fancy Technology
provider_slug: fancy-technology
slug: fancy-technology-domain-security
source_filename: fancy-technology-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fancy.tech\n  https: false\ndomains:\n- domain: fancy.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fancy-technology/refs/heads/main/security/fancy-technology-domain-security.yml
summary_line: DMARC
tags:
- Company
- Enterprise
---
