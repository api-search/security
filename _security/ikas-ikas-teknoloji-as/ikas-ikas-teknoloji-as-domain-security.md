---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ikas.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: ikas.dev
  spf: false
hosts:
- cert_expires: Sep 13 09:57:49 2026 GMT
  host: ikas.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 06:32:49 2026 GMT
  host: ikas.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 09:10:14 2026 GMT
  host: api.myikas.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ikas Ikas Teknoloji As Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ikas, IKAS Teknoloji AS, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Ikas, IKAS Teknoloji AS
provider_slug: ikas-ikas-teknoloji-as
slug: ikas-ikas-teknoloji-as-domain-security
source_filename: ikas-ikas-teknoloji-as-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ikas.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 09:57:49 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: ikas.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 06:32:49 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.myikas.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 09:10:14 2026 GMT\n  hsts: null\ndomains:\n- domain: ikas.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: ikas.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ikas-ikas-teknoloji-as/refs/heads/main/security/ikas-ikas-teknoloji-as-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- E-commerce
- Retail
- Storefront
- Orders
- Products
- Inventory
- GraphQL
- Webhooks
- OAuth
- SDK
- MCP
---
