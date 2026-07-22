---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: rupeek.com
  spf: true
hosts:
- host: www.rupeek.com
  https: false
kind: domain-security
layout: security
method: probed
name: Rupeek Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rupeek, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Rupeek
provider_slug: rupeek
slug: rupeek-domain-security
source_filename: rupeek-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rupeek.com\n  https: false\ndomains:\n- domain: rupeek.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rupeek/refs/heads/main/security/rupeek-domain-security.yml
summary_line: DMARC
tags:
- Company
- Consumer
- Fintech
- Lending
- Gold Loan
- Financial Services
- India
---
