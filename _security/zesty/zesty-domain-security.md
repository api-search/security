---
api_specs:
- filename: zesty-auth-api-openapi.yml
  format: yaml
  label: Zesty Auth API
  slug: auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zesty/refs/heads/main/openapi/zesty-auth-api-openapi.yml
- filename: zesty-accounts-api-openapi.yml
  format: yaml
  label: Zesty Accounts API
  slug: accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zesty/refs/heads/main/openapi/zesty-accounts-api-openapi.yml
- filename: zesty-instances-api-openapi.yml
  format: yaml
  label: Zesty Instances API
  slug: instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zesty/refs/heads/main/openapi/zesty-instances-api-openapi.yml
- filename: zesty-media-api-openapi.yml
  format: yaml
  label: Zesty Media API
  slug: media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zesty/refs/heads/main/openapi/zesty-media-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: zesty.io
  spf: true
hosts:
- cert_expires: Sep 14 08:42:59 2026 GMT
  host: docs.zesty.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 19 23:59:59 2027 GMT
  host: accounts.api.zesty.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 19 23:59:59 2027 GMT
  host: auth.api.zesty.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zesty Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zesty, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Zesty
provider_slug: zesty
slug: zesty-domain-security
source_filename: zesty-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.zesty.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:42:59 2026 GMT\n  hsts: null\n- host: accounts.api.zesty.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 23:59:59 2027 GMT\n  hsts: false\n- host: auth.api.zesty.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: zesty.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zesty/refs/heads/main/security/zesty-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- CMS
- Composable
- Content Management
- GraphQL
- Headless CMS
- Media
---
