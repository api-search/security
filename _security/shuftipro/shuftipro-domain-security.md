---
api_specs:
- filename: shuftipro-openapi.yml
  format: yaml
  label: Shufti Pro Verification API
  slug: shuftipro-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shuftipro/refs/heads/main/openapi/shuftipro-openapi.yml
- filename: shuftipro-openapi.yml
  format: yaml
  label: Shufti Pro KYB API
  slug: shuftipro-kyb-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shuftipro/refs/heads/main/openapi/shuftipro-openapi.yml
- filename: shuftipro-openapi.yml
  format: yaml
  label: Shufti Pro AML & Background Checks API
  slug: shuftipro-aml-background-checks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shuftipro/refs/heads/main/openapi/shuftipro-openapi.yml
- filename: shuftipro-openapi.yml
  format: yaml
  label: Shufti Pro Status API
  slug: shuftipro-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shuftipro/refs/heads/main/openapi/shuftipro-openapi.yml
- filename: shuftipro-openapi.yml
  format: yaml
  label: Shufti Pro Webhooks API
  slug: shuftipro-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shuftipro/refs/heads/main/openapi/shuftipro-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: shuftipro.com
  spf: true
hosts:
- cert_expires: Aug 29 08:45:16 2026 GMT
  host: shuftipro.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 28 09:40:26 2026 GMT
  host: developers.shuftipro.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 18:59:52 2026 GMT
  host: api.shuftipro.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Shuftipro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Shufti Pro, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Shufti Pro
provider_slug: shuftipro
slug: shuftipro-domain-security
source_filename: shuftipro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: shuftipro.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 08:45:16 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: developers.shuftipro.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 09:40:26 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.shuftipro.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 18:59:52 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: shuftipro.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shuftipro/refs/heads/main/security/shuftipro-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Identity Verification
- KYC
- KYB
- AML
- Compliance
---
