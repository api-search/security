---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: stableprice.com
  spf: true
hosts:
- host: stableprice.com
  https: false
kind: domain-security
layout: security
method: probed
name: Stable Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stable, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Stable
provider_slug: stable
slug: stable-domain-security
source_filename: stable-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: stableprice.com\n  https: false\ndomains:\n- domain: stableprice.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stable/refs/heads/main/security/stable-domain-security.yml
summary_line: DNSSEC · DMARC
tags:
- Company
- Insurance
- InsurTech
- FinTech
- Commodities
- Agriculture
- Risk Management
- Price Insurance
---
