---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Weebly REST API
  slug: weebly-api
  spec_type: OpenAPI
  url: https://dev.weebly.com/
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: weebly.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: weeblycloud.com
  spf: false
hosts:
- cert_expires: Sep  8 20:33:04 2026 GMT
  host: www.weebly.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 09:57:17 2026 GMT
  host: dev.weebly.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 03:28:45 2026 GMT
  host: api.weeblycloud.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Weebly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Weebly, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Weebly
provider_slug: weebly
slug: weebly-domain-security
source_filename: weebly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.weebly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 20:33:04 2026 GMT\n  hsts: false\n- host: dev.weebly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 09:57:17 2026 GMT\n  hsts: null\n- host: api.weeblycloud.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 03:28:45 2026 GMT\n  hsts: null\ndomains:\n- domain: weebly.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: weeblycloud.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/weebly/refs/heads/main/security/weebly-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Website Builder
- E-Commerce
- Blogging
- Sites
- Pages
- Products
- Orders
- Customers
- Square
---
