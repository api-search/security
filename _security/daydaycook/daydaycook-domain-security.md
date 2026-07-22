---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: daydaycook.com
  spf: true
hosts:
- cert_expires: Sep 18 23:13:45 2026 GMT
  host: daydaycook.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Daydaycook Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DayDayCook, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: DayDayCook
provider_slug: daydaycook
slug: daydaycook-domain-security
source_filename: daydaycook-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: daydaycook.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 23:13:45 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: daydaycook.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/daydaycook/refs/heads/main/security/daydaycook-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Food
- Recipes
- Cooking
- Media
- Content
- Consumer
- E-Commerce
---
