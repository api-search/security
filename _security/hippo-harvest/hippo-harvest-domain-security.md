---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: hippoharvest.com
  spf: true
hosts:
- cert_expires: Oct 18 13:11:58 2026 GMT
  host: www.hippoharvest.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hippo Harvest Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hippo Harvest, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Hippo Harvest
provider_slug: hippo-harvest
slug: hippo-harvest-domain-security
source_filename: hippo-harvest-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hippoharvest.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 13:11:58 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: hippoharvest.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hippo-harvest/refs/heads/main/security/hippo-harvest-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Agriculture
- Controlled Environment Agriculture
- Robotics
- Food and Beverage
- Sustainability
- Consumer Packaged Goods
---
