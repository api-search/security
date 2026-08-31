---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: zuoyebang.com
  spf: true
hosts:
- host: www.zuoyebang.com
  https: false
kind: domain-security
layout: security
method: probed
name: Zuoyebang Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zuoyebang, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Zuoyebang
provider_slug: zuoyebang
slug: zuoyebang-domain-security
source_filename: zuoyebang-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.zuoyebang.com\n  https: false\ndomains:\n- domain: zuoyebang.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zuoyebang/refs/heads/main/security/zuoyebang-domain-security.yml
summary_line: DMARC
tags:
- Company
- Edtech
- Education
- Online Learning
- Tutoring
- Consumer
- China
---
