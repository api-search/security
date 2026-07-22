---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: natalist.com
  spf: true
hosts:
- host: www.natalist.com
  https: false
kind: domain-security
layout: security
method: probed
name: Natalist Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Natalist, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Natalist
provider_slug: natalist
slug: natalist-domain-security
source_filename: natalist-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.natalist.com\n  https: false\ndomains:\n- domain: natalist.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/natalist/refs/heads/main/security/natalist-domain-security.yml
summary_line: DMARC
tags:
- Company
- Consumer
- Fertility
- Pregnancy
- Women's Health
- Consumer Health
- Ecommerce
---
