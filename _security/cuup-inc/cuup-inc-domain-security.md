---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: shopcuup.com
  spf: true
hosts:
- cert_expires: Nov 26 19:07:35 2026 GMT
  host: shopcuup.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cuup Inc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CUUP, Inc., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: CUUP, Inc.
provider_slug: cuup-inc
slug: cuup-inc-domain-security
source_filename: cuup-inc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: shopcuup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 19:07:35 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: shopcuup.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cuup-inc/refs/heads/main/security/cuup-inc-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Consumer
- Retail
- E-Commerce
- Apparel
- Intimates
- Direct-to-Consumer
- Fashion
---
