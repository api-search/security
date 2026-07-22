---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: crowdery.com
  spf: true
hosts:
- host: crowdery.com
  https: false
kind: domain-security
layout: security
method: probed
name: Crowdery Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Crowdery, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Crowdery
provider_slug: crowdery
slug: crowdery-domain-security
source_filename: crowdery-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: crowdery.com\n  https: false\ndomains:\n- domain: crowdery.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crowdery/refs/heads/main/security/crowdery-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Retail
- E-Commerce
- Consumer
- Marketplace
- Crowdsourcing
- Pre-Order
- Defunct
- No API
---
