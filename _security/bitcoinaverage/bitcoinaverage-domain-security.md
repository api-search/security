---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: bitcoinaverage.com
  spf: true
hosts:
- host: apiv2.bitcoinaverage.com
  https: false
kind: domain-security
layout: security
method: probed
name: Bitcoinaverage Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BitcoinAverage, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: BitcoinAverage
provider_slug: bitcoinaverage
slug: bitcoinaverage-domain-security
source_filename: bitcoinaverage-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apiv2.bitcoinaverage.com\n  https: false\ndomains:\n- domain: bitcoinaverage.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bitcoinaverage/refs/heads/main/security/bitcoinaverage-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Cryptocurrency
- Public APIs
---
