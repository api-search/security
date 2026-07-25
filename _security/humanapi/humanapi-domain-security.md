---
api_specs:
- filename: humanapi-admin-api-openapi.yml
  format: yaml
  label: HumanAPI admin API
  slug: humanapi-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/humanapi/refs/heads/main/openapi/humanapi-admin-api-openapi.yml
- filename: humanapi-connect-api-openapi.yml
  format: yaml
  label: HumanAPI connect API
  slug: humanapi-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/humanapi/refs/heads/main/openapi/humanapi-connect-api-openapi.yml
- filename: humanapi-orders-api-openapi.yml
  format: yaml
  label: HumanAPI orders API
  slug: humanapi-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/humanapi/refs/heads/main/openapi/humanapi-orders-api-openapi.yml
- filename: humanapi-reports-api-openapi.yml
  format: yaml
  label: HumanAPI reports API
  slug: humanapi-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/humanapi/refs/heads/main/openapi/humanapi-reports-api-openapi.yml
- filename: humanapi-resources-api-openapi.yml
  format: yaml
  label: HumanAPI resources API
  slug: humanapi-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/humanapi/refs/heads/main/openapi/humanapi-resources-api-openapi.yml
- filename: humanapi-subscriptions-api-openapi.yml
  format: yaml
  label: HumanAPI subscriptions API
  slug: humanapi-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/humanapi/refs/heads/main/openapi/humanapi-subscriptions-api-openapi.yml
- filename: humanapi-users-api-openapi.yml
  format: yaml
  label: HumanAPI users API
  slug: humanapi-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/humanapi/refs/heads/main/openapi/humanapi-users-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: humanapi.co
  spf: true
hosts:
- cert_expires: Nov  6 23:59:59 2026 GMT
  host: admin.humanapi.co
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov  6 23:59:59 2026 GMT
  host: auth.humanapi.co
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Humanapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HumanAPI, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: HumanAPI
provider_slug: humanapi
slug: humanapi-domain-security
source_filename: humanapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: admin.humanapi.co\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  6 23:59:59 2026 GMT\n  hsts: null\n- host: auth.humanapi.co\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  6 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: humanapi.co\n  dnssec: false\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/humanapi/refs/heads/main/security/humanapi-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Health
- Healthcare
- Health Data
- Medical Records
- Insurance
- Underwriting
- Wellness
- Data Aggregation
- Reports
- FHIR-adjacent
---
