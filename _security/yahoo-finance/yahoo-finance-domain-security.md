---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: yahoofinanceapi.com
  spf: true
hosts:
- host: www.yahoofinanceapi.com
  https: false
kind: domain-security
layout: security
method: probed
name: Yahoo Finance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Yahoo Finance, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Yahoo Finance
provider_slug: yahoo-finance
slug: yahoo-finance-domain-security
source_filename: yahoo-finance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.yahoofinanceapi.com\n  https: false\ndomains:\n- domain: yahoofinanceapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yahoo-finance/refs/heads/main/security/yahoo-finance-domain-security.yml
summary_line: DMARC
tags:
- Finance
- Public APIs
---
