---
api_specs:
- filename: parcellab-events-api-openapi.yml
  format: yaml
  label: parcelLab Events API
  slug: parcellab-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parcellab/openapi/parcellab-events-api-openapi.yml
- filename: parcellab-place-info-api-openapi.yml
  format: yaml
  label: parcelLab Place Info API
  slug: parcellab-place-info-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parcellab/openapi/parcellab-place-info-api-openapi.yml
- filename: parcellab-promise-api-openapi.yml
  format: yaml
  label: parcelLab Promise API
  slug: parcellab-promise-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parcellab/openapi/parcellab-promise-api-openapi.yml
- filename: parcellab-agents-api-openapi.yml
  format: yaml
  label: parcelLab Agents API
  slug: parcellab-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parcellab/openapi/parcellab-agents-api-openapi.yml
- filename: parcellab-apps-api-openapi.yml
  format: yaml
  label: parcelLab Apps API
  slug: parcellab-apps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parcellab/openapi/parcellab-apps-api-openapi.yml
- filename: parcellab-campaign-api-openapi.yml
  format: yaml
  label: parcelLab Campaign API
  slug: parcellab-campaign-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parcellab/openapi/parcellab-campaign-api-openapi.yml
- filename: parcellab-customer-portals-api-openapi.yml
  format: yaml
  label: parcelLab Customer Portals API
  slug: parcellab-customer-portals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parcellab/openapi/parcellab-customer-portals-api-openapi.yml
- filename: parcellab-order-api-openapi.yml
  format: yaml
  label: parcelLab Order API
  slug: parcellab-order-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parcellab/openapi/parcellab-order-api-openapi.yml
- filename: parcellab-order-status-page-theme-api-openapi.yml
  format: yaml
  label: parcelLab Order Status Page Theme API
  slug: parcellab-order-status-page-theme-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parcellab/openapi/parcellab-order-status-page-theme-api-openapi.yml
- filename: parcellab-return-configuration-set-api-openapi.yml
  format: yaml
  label: parcelLab Return Configuration Set API
  slug: parcellab-return-configuration-set-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parcellab/openapi/parcellab-return-configuration-set-api-openapi.yml
- filename: parcellab-return-registration-api-openapi.yml
  format: yaml
  label: parcelLab Return Registration API
  slug: parcellab-return-registration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parcellab/openapi/parcellab-return-registration-api-openapi.yml
- filename: parcellab-size-recommender-api-openapi.yml
  format: yaml
  label: parcelLab Size Recommender API
  slug: parcellab-size-recommender-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parcellab/openapi/parcellab-size-recommender-api-openapi.yml
- filename: parcellab-survey-api-openapi.yml
  format: yaml
  label: parcelLab Survey API
  slug: parcellab-survey-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parcellab/openapi/parcellab-survey-api-openapi.yml
- filename: parcellab-theme-api-openapi.yml
  format: yaml
  label: parcelLab Theme API
  slug: parcellab-theme-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parcellab/openapi/parcellab-theme-api-openapi.yml
- filename: parcellab-translation-api-openapi.yml
  format: yaml
  label: parcelLab Translation API
  slug: parcellab-translation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parcellab/openapi/parcellab-translation-api-openapi.yml
- filename: parcellab-voucher-api-openapi.yml
  format: yaml
  label: parcelLab Voucher API
  slug: parcellab-voucher-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parcellab/openapi/parcellab-voucher-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "awstrust.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: parcellab.com
  spf: true
hosts:
- cert_expires: Jan  4 23:53:04 2027 GMT
  host: parcellab.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 22 23:59:59 2027 GMT
  host: agents.parcellab.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 25 17:21:46 2026 GMT
  host: docs.parcellab.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: parcelLab Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for parcelLab, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: parcelLab
provider_slug: parcellab
slug: parcellab-domain-security
source_filename: parcellab-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: parcellab.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 23:53:04 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: agents.parcellab.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 22 23:59:59 2027 GMT\n  hsts: null\n- host: docs.parcellab.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 17:21:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: parcellab.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/parcellab/security/parcellab-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Post-Purchase
- E-Commerce
- Tracking
- Returns
- Shipping
- Delivery
- Customer Experience
- Logistics
- Communications
- Germany
---
