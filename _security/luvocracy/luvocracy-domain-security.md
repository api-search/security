---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: luvocracy.com
  spf: true
hosts:
- host: luvocracy.com
  https: false
kind: domain-security
layout: security
method: probed
name: Luvocracy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Luvocracy *, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Luvocracy *
provider_slug: luvocracy
slug: luvocracy-domain-security
source_filename: luvocracy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: luvocracy.com\n  https: false\ndomains:\n- domain: luvocracy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/luvocracy/refs/heads/main/security/luvocracy-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Consumer
- Social Commerce
- Marketplace
- Shopping
- Recommendations
- Acquired
- Defunct
---
