---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: heyo.com
  spf: true
hosts:
- cert_expires: Nov 21 14:35:15 2026 GMT
  host: heyo.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Heyo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Heyo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Heyo
provider_slug: heyo
slug: heyo-domain-security
source_filename: heyo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: heyo.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 21 14:35:15 2026 GMT\n  hsts: false\ndomains:\n- domain: heyo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/heyo/refs/heads/main/security/heyo-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Marketing
- Social Media
- Promotions
- Contests
- Sweepstakes
- Giveaways
- Lead Generation
- Email Marketing
- Campaigns
---
