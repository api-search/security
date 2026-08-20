---
api_specs:
- filename: hooklogic-criteo-accounts-api-openapi.yml
  format: yaml
  label: HookLogic (Criteo) Accounts API
  slug: hooklogic-criteo-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hooklogic-criteo/refs/heads/main/openapi/hooklogic-criteo-accounts-api-openapi.yml
- filename: hooklogic-criteo-analytics-api-openapi.yml
  format: yaml
  label: HookLogic (Criteo) Analytics API
  slug: hooklogic-criteo-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hooklogic-criteo/refs/heads/main/openapi/hooklogic-criteo-analytics-api-openapi.yml
- filename: hooklogic-criteo-audience-api-openapi.yml
  format: yaml
  label: HookLogic (Criteo) Audience API
  slug: hooklogic-criteo-audience-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hooklogic-criteo/refs/heads/main/openapi/hooklogic-criteo-audience-api-openapi.yml
- filename: hooklogic-criteo-balance-api-openapi.yml
  format: yaml
  label: HookLogic (Criteo) Balance API
  slug: hooklogic-criteo-balance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hooklogic-criteo/refs/heads/main/openapi/hooklogic-criteo-balance-api-openapi.yml
- filename: hooklogic-criteo-billing-api-openapi.yml
  format: yaml
  label: HookLogic (Criteo) Billing API
  slug: hooklogic-criteo-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hooklogic-criteo/refs/heads/main/openapi/hooklogic-criteo-billing-api-openapi.yml
- filename: hooklogic-criteo-campaign-api-openapi.yml
  format: yaml
  label: HookLogic (Criteo) Campaign API
  slug: hooklogic-criteo-campaign-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hooklogic-criteo/refs/heads/main/openapi/hooklogic-criteo-campaign-api-openapi.yml
- filename: hooklogic-criteo-catalog-api-openapi.yml
  format: yaml
  label: HookLogic (Criteo) Catalog API
  slug: hooklogic-criteo-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hooklogic-criteo/refs/heads/main/openapi/hooklogic-criteo-catalog-api-openapi.yml
- filename: hooklogic-criteo-gateway-api-openapi.yml
  format: yaml
  label: HookLogic (Criteo) Gateway API
  slug: hooklogic-criteo-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hooklogic-criteo/refs/heads/main/openapi/hooklogic-criteo-gateway-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  - 0 issue "pki.goog"
  - 0 issue "godaddy.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: criteo.com
  spf: true
hosts:
- cert_expires: Sep 28 13:16:40 2026 GMT
  host: developers.criteo.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: api.criteo.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hooklogic Criteo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HookLogic (Criteo), probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: HookLogic (Criteo)
provider_slug: hooklogic-criteo
slug: hooklogic-criteo-domain-security
source_filename: hooklogic-criteo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.criteo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 13:16:40 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.criteo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: criteo.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hooklogic-criteo/refs/heads/main/security/hooklogic-criteo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Commerce
- Retail Media
- Advertising
- E-Commerce
- Marketing
- Retail
---
