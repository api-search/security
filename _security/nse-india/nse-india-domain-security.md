---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: nse-india.com
  spf: true
hosts:
- host: nse-india.com
  https: false
kind: domain-security
layout: security
method: probed
name: Nse India Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nse-india, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Nse-india
provider_slug: nse-india
slug: nse-india-domain-security
source_filename: nse-india-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nse-india.com\n  https: false\ndomains:\n- domain: nse-india.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nse-india/refs/heads/main/security/nse-india-domain-security.yml
summary_line: DNSSEC · DMARC
tags:
- Company
- Stock Exchange
- Financial Services
- Market Data
- Capital Markets
- Trading
- India
---
