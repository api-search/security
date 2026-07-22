---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: rizefs.com
  spf: true
hosts:
- host: rizefs.com
  https: false
kind: domain-security
layout: security
method: probed
name: Rize Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rize, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Rize
provider_slug: rize
slug: rize-domain-security
source_filename: rize-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rizefs.com\n  https: false\ndomains:\n- domain: rizefs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rize/refs/heads/main/security/rize-domain-security.yml
summary_line: DMARC
tags:
- Company
- Fintech
- Banking
- Banking as a Service
- Embedded Finance
- Payments
- Financial Services
- Brokerage
---
