---
api_specs:
- filename: xoomar-com-companies-api-openapi.yml
  format: yaml
  label: XOOMAR Companies API
  slug: xoomar-com-companies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/xoomar-com/openapi/xoomar-com-companies-api-openapi.yml
- filename: xoomar-com-crypto-api-openapi.yml
  format: yaml
  label: XOOMAR Crypto API
  slug: xoomar-com-crypto-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/xoomar-com/openapi/xoomar-com-crypto-api-openapi.yml
- filename: xoomar-com-macro-api-openapi.yml
  format: yaml
  label: XOOMAR Macro API
  slug: xoomar-com-macro-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/xoomar-com/openapi/xoomar-com-macro-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: xoomar.com
  spf: true
hosts:
- cert_expires: Jan  2 04:57:25 2027 GMT
  host: xoomar.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: XOOMAR Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for XOOMAR, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: XOOMAR
provider_slug: xoomar-com
slug: xoomar-com-domain-security
source_filename: xoomar-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: xoomar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 04:57:25 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: xoomar.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/xoomar-com/security/xoomar-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Capital Markets
- Data
- Financial Services
- Software
---
