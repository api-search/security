---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: arda.finance
  spf: true
hosts:
- host: arda.finance
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Arda Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Arda, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Arda
provider_slug: arda
slug: arda-domain-security
source_filename: arda-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: arda.finance\n  https: false\ndomains:\n- domain: arda.finance\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/arda/security/arda-domain-security.yml
summary_line: DNSSEC · DMARC
tags:
- Company
- FinTech
- API
- DigitalAssets
- Trading
---
