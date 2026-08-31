---
api_specs:
- filename: zesty-instances-api-openapi.yml
  format: yaml
  label: Zesty Instances API
  slug: instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zesty/refs/heads/main/openapi/zesty-instances-api-openapi.yml
- filename: zesty-apps-api-openapi.yml
  format: yaml
  label: Zesty Apps API
  slug: zesty-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zesty/refs/heads/main/openapi/zesty-apps-api-openapi.yml
- filename: zesty-authentication-api-openapi.yml
  format: yaml
  label: Zesty Authentication API
  slug: zesty-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zesty/refs/heads/main/openapi/zesty-authentication-api-openapi.yml
- filename: zesty-bins-api-openapi.yml
  format: yaml
  label: Zesty Bins API
  slug: zesty-bins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zesty/refs/heads/main/openapi/zesty-bins-api-openapi.yml
- filename: zesty-files-api-openapi.yml
  format: yaml
  label: Zesty Files API
  slug: zesty-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zesty/refs/heads/main/openapi/zesty-files-api-openapi.yml
- filename: zesty-groups-api-openapi.yml
  format: yaml
  label: Zesty Groups API
  slug: zesty-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zesty/refs/heads/main/openapi/zesty-groups-api-openapi.yml
- filename: zesty-password-api-openapi.yml
  format: yaml
  label: Zesty Password API
  slug: zesty-password-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zesty/refs/heads/main/openapi/zesty-password-api-openapi.yml
- filename: zesty-resolver-api-openapi.yml
  format: yaml
  label: Zesty Resolver API
  slug: zesty-resolver-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zesty/refs/heads/main/openapi/zesty-resolver-api-openapi.yml
- filename: zesty-roles-api-openapi.yml
  format: yaml
  label: Zesty Roles API
  slug: zesty-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zesty/refs/heads/main/openapi/zesty-roles-api-openapi.yml
- filename: zesty-teams-api-openapi.yml
  format: yaml
  label: Zesty Teams API
  slug: zesty-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zesty/refs/heads/main/openapi/zesty-teams-api-openapi.yml
- filename: zesty-tokens-api-openapi.yml
  format: yaml
  label: Zesty Tokens API
  slug: zesty-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zesty/refs/heads/main/openapi/zesty-tokens-api-openapi.yml
- filename: zesty-users-api-openapi.yml
  format: yaml
  label: Zesty Users API
  slug: zesty-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zesty/refs/heads/main/openapi/zesty-users-api-openapi.yml
- filename: zesty-webhooks-api-openapi.yml
  format: yaml
  label: Zesty Webhooks API
  slug: zesty-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zesty/refs/heads/main/openapi/zesty-webhooks-api-openapi.yml
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
