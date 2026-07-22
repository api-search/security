---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: eqrx.com
  spf: true
hosts:
- host: eqrx.com
  https: false
kind: domain-security
layout: security
method: probed
name: Eqrx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EQRx, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: EQRx
provider_slug: eqrx
slug: eqrx-domain-security
source_filename: eqrx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: eqrx.com\n  https: false\ndomains:\n- domain: eqrx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eqrx/refs/heads/main/security/eqrx-domain-security.yml
summary_line: DMARC
tags:
- Company
- Biopharmaceutical
- Pharmaceuticals
- Biotechnology
- Oncology
- Drug Development
- Life Sciences
- Healthcare
---
