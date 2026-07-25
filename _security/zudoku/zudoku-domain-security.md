---
api_specs:
- filename: zudoku-configuration-api-openapi.yml
  format: yaml
  label: Zudoku Configuration API
  slug: configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zudoku/refs/heads/main/openapi/zudoku-configuration-api-openapi.yml
- filename: zudoku-api-references-api-openapi.yml
  format: yaml
  label: Zudoku API References API
  slug: zudoku-api-references-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zudoku/refs/heads/main/openapi/zudoku-api-references-api-openapi.yml
- filename: zudoku-authentication-api-openapi.yml
  format: yaml
  label: Zudoku Authentication API
  slug: zudoku-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zudoku/refs/heads/main/openapi/zudoku-authentication-api-openapi.yml
- filename: zudoku-navigation-api-openapi.yml
  format: yaml
  label: Zudoku Navigation API
  slug: zudoku-navigation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zudoku/refs/heads/main/openapi/zudoku-navigation-api-openapi.yml
- filename: zudoku-plugins-api-openapi.yml
  format: yaml
  label: Zudoku Plugins API
  slug: zudoku-plugins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zudoku/refs/heads/main/openapi/zudoku-plugins-api-openapi.yml
- filename: zudoku-theming-api-openapi.yml
  format: yaml
  label: Zudoku Theming API
  slug: zudoku-theming-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zudoku/refs/heads/main/openapi/zudoku-theming-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: zudoku.dev
  spf: false
hosts:
- cert_expires: Aug 15 12:17:22 2026 GMT
  host: zudoku.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zudoku Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zudoku, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Zudoku
provider_slug: zudoku
slug: zudoku-domain-security
source_filename: zudoku-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zudoku.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 12:17:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: zudoku.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zudoku/refs/heads/main/security/zudoku-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Developer Tools
- Documentation
---
