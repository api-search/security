---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: mamut.com
  spf: true
hosts:
- host: www.mamut.com
  https: false
kind: domain-security
layout: security
method: probed
name: Mamut Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mamut, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Mamut
provider_slug: mamut
slug: mamut-domain-security
source_filename: mamut-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mamut.com\n  https: false\ndomains:\n- domain: mamut.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mamut/refs/heads/main/security/mamut-domain-security.yml
summary_line: DNSSEC
tags:
- Company
- Enterprise
- Accounting
- ERP
- Business Software
- SMB
- Norway
- Visma
---
