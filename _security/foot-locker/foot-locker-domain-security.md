---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: foot-locker.com
  spf: true
hosts:
- host: www.foot-locker.com
  https: false
kind: domain-security
layout: security
method: probed
name: Foot Locker Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Foot Locker, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Foot Locker
provider_slug: foot-locker
slug: foot-locker-domain-security
source_filename: foot-locker-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.foot-locker.com\n  https: false\ndomains:\n- domain: foot-locker.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/foot-locker/refs/heads/main/security/foot-locker-domain-security.yml
summary_line: DMARC
tags:
- Fortune 500
- Retail
- Footwear
- Apparel
- E-Commerce
---
