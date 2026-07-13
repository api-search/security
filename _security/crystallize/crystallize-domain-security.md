---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: crystallize.com
  spf: true
hosts:
- cert_expires: Sep 26 05:49:04 2026 GMT
  host: crystallize.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 23:59:59 2026 GMT
  host: api.crystallize.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 22 15:40:15 2026 GMT
  host: shop-api.crystallize.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Crystallize Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Crystallize, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Crystallize
provider_slug: crystallize
slug: crystallize-domain-security
source_filename: crystallize-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: crystallize.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 05:49:04 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.crystallize.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  3 23:59:59 2026 GMT\n  hsts: null\n- host: shop-api.crystallize.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 15:40:15 2026 GMT\n  hsts: false\ndomains:\n- domain: crystallize.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crystallize/refs/heads/main/security/crystallize-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Commerce
- Headless Commerce
- Product Information Management
- PIM
- GraphQL
- Catalog
- Search
- Orders
- Subscriptions
---
