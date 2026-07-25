---
api_specs:
- filename: wove-authentication-api-openapi.yml
  format: yaml
  label: Wove Authentication API
  slug: wove-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wove/refs/heads/main/openapi/wove-authentication-api-openapi.yml
- filename: wove-documents-api-openapi.yml
  format: yaml
  label: Wove Documents API
  slug: wove-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wove/refs/heads/main/openapi/wove-documents-api-openapi.yml
- filename: wove-query-bank-api-openapi.yml
  format: yaml
  label: Wove Query Bank API
  slug: wove-query-bank-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wove/refs/heads/main/openapi/wove-query-bank-api-openapi.yml
- filename: wove-rates-api-openapi.yml
  format: yaml
  label: Wove Rates API
  slug: wove-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wove/refs/heads/main/openapi/wove-rates-api-openapi.yml
- filename: wove-shipments-api-openapi.yml
  format: yaml
  label: Wove Shipments API
  slug: wove-shipments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wove/refs/heads/main/openapi/wove-shipments-api-openapi.yml
- filename: wove-sources-api-openapi.yml
  format: yaml
  label: Wove Sources API
  slug: wove-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wove/refs/heads/main/openapi/wove-sources-api-openapi.yml
- filename: wove-tariffs-api-openapi.yml
  format: yaml
  label: Wove Tariffs API
  slug: wove-tariffs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wove/refs/heads/main/openapi/wove-tariffs-api-openapi.yml
- filename: wove-testing-api-openapi.yml
  format: yaml
  label: Wove Testing API
  slug: wove-testing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wove/refs/heads/main/openapi/wove-testing-api-openapi.yml
- filename: wove-tms-organizations-api-openapi.yml
  format: yaml
  label: Wove TMS Organizations API
  slug: wove-tms-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wove/refs/heads/main/openapi/wove-tms-organizations-api-openapi.yml
- filename: wove-webhooks-api-openapi.yml
  format: yaml
  label: Wove Webhooks API
  slug: wove-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wove/refs/heads/main/openapi/wove-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: wove.com
  spf: true
hosts:
- cert_expires: Sep 10 01:59:57 2026 GMT
  host: wove.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 04:46:32 2026 GMT
  host: api.wove.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: staging-api.wove.com
  https: false
kind: domain-security
layout: security
method: probed
name: Wove Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wove, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Wove
provider_slug: wove
slug: wove-domain-security
source_filename: wove-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wove.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 01:59:57 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.wove.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 04:46:32 2026 GMT\n  hsts: null\n- host: staging-api.wove.com\n  https: false\ndomains:\n- domain: wove.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wove/refs/heads/main/security/wove-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
---
