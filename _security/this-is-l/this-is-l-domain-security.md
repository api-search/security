---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: thisisl.com
  spf: true
hosts:
- cert_expires: Aug 30 23:59:59 2026 GMT
  host: thisisl.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: This Is L Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for This Is L., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: This Is L.
provider_slug: this-is-l
slug: this-is-l-domain-security
source_filename: this-is-l-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: thisisl.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 30 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: thisisl.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/this-is-l/refs/heads/main/security/this-is-l-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Consumer Packaged Goods
- E-Commerce
- Personal Care
- Menstrual Care
- Organic
- Retail
- Direct to Consumer
---
