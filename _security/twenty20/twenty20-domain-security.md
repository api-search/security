---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: twenty20.com
  spf: true
hosts:
- host: www.twenty20.com
  https: false
kind: domain-security
layout: security
method: probed
name: Twenty20 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Twenty20, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Twenty20
provider_slug: twenty20
slug: twenty20-domain-security
source_filename: twenty20-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.twenty20.com\n  https: false\ndomains:\n- domain: twenty20.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/twenty20/refs/heads/main/security/twenty20-domain-security.yml
summary_line: DMARC
tags:
- Company
- Stock Photos
- Photography
- Creative Assets
- Marketplace
- Acquired
---
