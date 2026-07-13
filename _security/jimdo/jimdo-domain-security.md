---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Jimdo API
  slug: jimdo-api
  spec_type: OpenAPI
  url: https://dev.jimdoweb.com/
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: jimdo.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: jimdoweb.com
  spf: false
hosts:
- cert_expires: Aug 29 17:57:18 2026 GMT
  host: www.jimdo.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 18:57:33 2026 GMT
  host: dev.jimdoweb.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.jimdo.com
  https: false
kind: domain-security
layout: security
method: probed
name: Jimdo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jimdo, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Jimdo
provider_slug: jimdo
slug: jimdo-domain-security
source_filename: jimdo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.jimdo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 17:57:18 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n- host: dev.jimdoweb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 18:57:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.jimdo.com\n  https: false\ndomains:\n- domain: jimdo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: jimdoweb.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jimdo/refs/heads/main/security/jimdo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Website Builder
- Ecommerce
- CMS
- Small Business
- Online Store
- Blog
---
