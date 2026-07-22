---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: hhgregg.com
  spf: true
hosts:
- cert_expires: Aug 30 01:06:01 2026 GMT
  host: www.hhgregg.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hhgregg Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for hhgregg, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: hhgregg
provider_slug: hhgregg
slug: hhgregg-domain-security
source_filename: hhgregg-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hhgregg.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 01:06:01 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: hhgregg.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hhgregg/refs/heads/main/security/hhgregg-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Appliances
- Electronics
- E-Commerce
- Retail
---
