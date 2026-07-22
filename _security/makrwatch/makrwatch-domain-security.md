---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: makrwatch.com
  spf: true
hosts:
- cert_expires: Sep 11 15:51:00 2026 GMT
  host: www.makrwatch.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Makrwatch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Makrwatch, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Makrwatch
provider_slug: makrwatch
slug: makrwatch-domain-security
source_filename: makrwatch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.makrwatch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 15:51:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: makrwatch.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/makrwatch/refs/heads/main/security/makrwatch-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Creator Economy
- Influencer Marketing
- Sponsorship
- Marketplace
- Advertising
- Content Creators
- Brand Deals
---
