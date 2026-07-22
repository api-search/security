---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: herb.co
  spf: true
hosts:
- cert_expires: Sep 25 07:33:48 2026 GMT
  host: herb.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Herb Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Herb, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Herb
provider_slug: herb
slug: herb-domain-security
source_filename: herb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: herb.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 07:33:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: herb.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/herb/refs/heads/main/security/herb-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cannabis
- Media
- Content
- E-commerce
- Marketplace
- Education
- Lifestyle
---
