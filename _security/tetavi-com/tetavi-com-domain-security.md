---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tetavi.com
  spf: true
hosts:
- host: www.tetavi.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Tetavi Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Yoom (fka Tetavi), probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Yoom (fka Tetavi)
provider_slug: tetavi-com
slug: tetavi-com-domain-security
source_filename: tetavi-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tetavi.com\n  https: false\ndomains:\n- domain: tetavi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/tetavi-com/security/tetavi-com-domain-security.yml
summary_line: DMARC
tags:
- Company
- FinTech
- Payments
- API
- Platform
- Mobile
---
