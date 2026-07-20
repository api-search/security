---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: dovetail.com
  spf: true
hosts:
- cert_expires: Nov  5 23:59:59 2026 GMT
  host: dovetail.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 21 09:03:34 2026 GMT
  host: developers.dovetail.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dovetail Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dovetail, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Dovetail
provider_slug: dovetail
slug: dovetail-domain-security
source_filename: dovetail-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dovetail.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developers.dovetail.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 09:03:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: dovetail.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dovetail/refs/heads/main/security/dovetail-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Consumer
- Customer Research
- User Research
- Customer Insights
- Customer Feedback
- Research Repository
- Analytics
- AI
- Product Management
---
