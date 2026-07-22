---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cheerfy.com
  spf: true
hosts:
- cert_expires: Oct 22 13:00:10 2026 GMT
  host: cheerfy.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Cheerfy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cheerfy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cheerfy
provider_slug: cheerfy
slug: cheerfy-domain-security
source_filename: cheerfy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cheerfy.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 22 13:00:10 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: cheerfy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cheerfy/refs/heads/main/security/cheerfy-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Restaurants
- Hospitality
- CRM
- Loyalty
- Customer Engagement
- Marketing Automation
- Online Ordering
- Payments
---
