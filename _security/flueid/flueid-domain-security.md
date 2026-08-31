---
api_specs:
- filename: flueid-account-api-openapi.yml
  format: yaml
  label: Flueid Account API
  slug: flueid-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flueid/refs/heads/main/openapi/flueid-account-api-openapi.yml
- filename: flueid-accountpartner-api-openapi.yml
  format: yaml
  label: Flueid Account Partner API
  slug: flueid-accountpartner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flueid/refs/heads/main/openapi/flueid-accountpartner-api-openapi.yml
- filename: flueid-clientcompanies-api-openapi.yml
  format: yaml
  label: Flueid Client Companies API
  slug: flueid-clientcompanies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flueid/refs/heads/main/openapi/flueid-clientcompanies-api-openapi.yml
- filename: flueid-documents-api-openapi.yml
  format: yaml
  label: Flueid Documents API
  slug: flueid-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flueid/refs/heads/main/openapi/flueid-documents-api-openapi.yml
- filename: flueid-farms-api-openapi.yml
  format: yaml
  label: Flueid Farms API
  slug: flueid-farms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flueid/refs/heads/main/openapi/flueid-farms-api-openapi.yml
- filename: flueid-neworders-api-openapi.yml
  format: yaml
  label: Flueid New Orders API
  slug: flueid-neworders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flueid/refs/heads/main/openapi/flueid-neworders-api-openapi.yml
- filename: flueid-orderdocumentsettings-api-openapi.yml
  format: yaml
  label: Flueid Order Document Settings API
  slug: flueid-orderdocumentsettings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flueid/refs/heads/main/openapi/flueid-orderdocumentsettings-api-openapi.yml
- filename: flueid-orderevents-api-openapi.yml
  format: yaml
  label: Flueid Order Events API
  slug: flueid-orderevents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flueid/refs/heads/main/openapi/flueid-orderevents-api-openapi.yml
- filename: flueid-orderoptions-api-openapi.yml
  format: yaml
  label: Flueid Order Options API
  slug: flueid-orderoptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flueid/refs/heads/main/openapi/flueid-orderoptions-api-openapi.yml
- filename: flueid-orders-api-openapi.yml
  format: yaml
  label: Flueid Orders API
  slug: flueid-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flueid/refs/heads/main/openapi/flueid-orders-api-openapi.yml
- filename: flueid-partnerordersettings-api-openapi.yml
  format: yaml
  label: Flueid Partner Order Settings API
  slug: flueid-partnerordersettings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flueid/refs/heads/main/openapi/flueid-partnerordersettings-api-openapi.yml
- filename: flueid-partners-api-openapi.yml
  format: yaml
  label: Flueid Partners API
  slug: flueid-partners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flueid/refs/heads/main/openapi/flueid-partners-api-openapi.yml
- filename: flueid-permissions-api-openapi.yml
  format: yaml
  label: Flueid Permissions API
  slug: flueid-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flueid/refs/heads/main/openapi/flueid-permissions-api-openapi.yml
- filename: flueid-propertydata-api-openapi.yml
  format: yaml
  label: Flueid Property Data API
  slug: flueid-propertydata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flueid/refs/heads/main/openapi/flueid-propertydata-api-openapi.yml
- filename: flueid-public-api-openapi.yml
  format: yaml
  label: Flueid Public API
  slug: flueid-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flueid/refs/heads/main/openapi/flueid-public-api-openapi.yml
- filename: flueid-settings-api-openapi.yml
  format: yaml
  label: Flueid Settings API
  slug: flueid-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flueid/refs/heads/main/openapi/flueid-settings-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: flueid.com
  spf: true
hosts:
- cert_expires: Nov 30 23:59:59 2026 GMT
  host: www.flueid.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  7 23:59:59 2026 GMT
  host: pro.flueid.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 20 23:59:59 2027 GMT
  host: api.pro.flueid.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Flueid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flueid, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Flueid
provider_slug: flueid
slug: flueid-domain-security
source_filename: flueid-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.flueid.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 23:59:59 2026 GMT\n  hsts: false\n- host: pro.flueid.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.pro.flueid.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 20 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: flueid.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flueid/refs/heads/main/security/flueid-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Real-Estate
- Title Insurance
- Mortgage
- Property Data
- Verification of Title
- Financial-Services
- Lending
- PropTech
- Settlement Services
---
