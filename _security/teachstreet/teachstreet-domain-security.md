---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: teachstreet.com
  spf: true
hosts:
- host: teachstreet.com
  https: false
kind: domain-security
layout: security
method: probed
name: Teachstreet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TeachStreet, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: TeachStreet
provider_slug: teachstreet
slug: teachstreet-domain-security
source_filename: teachstreet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: teachstreet.com\n  https: false\ndomains:\n- domain: teachstreet.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/teachstreet/refs/heads/main/security/teachstreet-domain-security.yml
summary_line: DMARC
tags:
- Company
- Education
- Online Learning
- Marketplace
- Classes
- Defunct
---
