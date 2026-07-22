---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: getroi.app
  spf: true
hosts:
- host: getroi.app
  https: false
kind: domain-security
layout: security
method: probed
name: Vegafund Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vegafund, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Vegafund
provider_slug: vegafund
slug: vegafund-domain-security
source_filename: vegafund-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getroi.app\n  https: false\ndomains:\n- domain: getroi.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vegafund/refs/heads/main/security/vegafund-domain-security.yml
summary_line: DMARC
tags:
- Company
- Fintech
- Investing
- Personal Finance
- Artificial Intelligence
- Acquired
---
