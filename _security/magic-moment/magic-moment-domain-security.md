---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: magicmoment.jp
  spf: true
hosts:
- cert_expires: Sep 24 10:20:01 2026 GMT
  host: www.magicmoment.jp
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Magic Moment Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Magic Moment, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Magic Moment
provider_slug: magic-moment
slug: magic-moment-domain-security
source_filename: magic-moment-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.magicmoment.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 10:20:01 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: magicmoment.jp\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/magic-moment/refs/heads/main/security/magic-moment-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Enterprise
- Sales
- Artificial Intelligence
- CRM
- Sales Automation
- SaaS
- Japan
---
