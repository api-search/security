---
api_specs:
- filename: powershop-data-holder-customers-api-openapi.yml
  format: yaml
  label: Powershop Data Holder Customers API
  slug: powershop-data-holder-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powershop/refs/heads/main/openapi/powershop-data-holder-customers-api-openapi.yml
- filename: powershop-data-holder-operations-api-openapi.yml
  format: yaml
  label: Powershop Data Holder Operations API
  slug: powershop-data-holder-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powershop/refs/heads/main/openapi/powershop-data-holder-operations-api-openapi.yml
- filename: powershop-distributed-energy-resources-api-openapi.yml
  format: yaml
  label: Powershop Distributed Energy Resources API
  slug: powershop-distributed-energy-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powershop/refs/heads/main/openapi/powershop-distributed-energy-resources-api-openapi.yml
- filename: powershop-electricity-service-points-api-openapi.yml
  format: yaml
  label: Powershop Electricity Service Points API
  slug: powershop-electricity-service-points-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powershop/refs/heads/main/openapi/powershop-electricity-service-points-api-openapi.yml
- filename: powershop-electricity-usage-api-openapi.yml
  format: yaml
  label: Powershop Electricity Usage API
  slug: powershop-electricity-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powershop/refs/heads/main/openapi/powershop-electricity-usage-api-openapi.yml
- filename: powershop-energy-account-balances-api-openapi.yml
  format: yaml
  label: Powershop Energy Account Balances API
  slug: powershop-energy-account-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powershop/refs/heads/main/openapi/powershop-energy-account-balances-api-openapi.yml
- filename: powershop-energy-account-billing-api-openapi.yml
  format: yaml
  label: Powershop Energy Account Billing API
  slug: powershop-energy-account-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powershop/refs/heads/main/openapi/powershop-energy-account-billing-api-openapi.yml
- filename: powershop-energy-accounts-api-openapi.yml
  format: yaml
  label: Powershop Energy Accounts API
  slug: powershop-energy-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powershop/refs/heads/main/openapi/powershop-energy-accounts-api-openapi.yml
- filename: powershop-energy-plans-api-openapi.yml
  format: yaml
  label: Powershop Energy Plans API
  slug: powershop-energy-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powershop/refs/heads/main/openapi/powershop-energy-plans-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: powershop.com.au
  spf: true
- caa:
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "awstrust.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazonaws.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: energymadeeasy.gov.au
  spf: true
hosts:
- cert_expires: Nov 21 23:59:59 2026 GMT
  host: www.powershop.com.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 31 23:59:59 2027 GMT
  host: cdr.energymadeeasy.gov.au
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 18 23:59:59 2026 GMT
  host: public.cdr.powershop.com.au
  hsts: null
  hsts_note: 'The probe records null because the host root returns an nginx 404 with no security headers. A GET of a real CDS endpoint on the same host (/cds-au/v1/discovery/status) does return strict-transport-security: max-age=63072000; includeSubDomains, plus x-content-type-options: nosniff and x-frame-options: DENY. HSTS is present on the API responses that matter.'
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Powershop Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Powershop, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Powershop
provider_slug: powershop
slug: powershop-domain-security
source_filename: powershop-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.powershop.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: cdr.energymadeeasy.gov.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 23:59:59 2027 GMT\n  hsts: null\n- host: public.cdr.powershop.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 23:59:59 2026 GMT\n  hsts: null\n  hsts_note: >-\n    The probe records null because the host root returns an nginx 404 with no\n    security headers. A GET of a real CDS endpoint on the same host\n    (/cds-au/v1/discovery/status) does return\n    strict-transport-security: max-age=63072000; includeSubDomains, plus\n    x-content-type-options: nosniff and x-frame-options: DENY. HSTS is present on\n    the API responses that matter.\ndomains:\n- domain: powershop.com.au\n  dnssec: true\n  caa:\n\
  \  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: energymadeeasy.gov.au\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/powershop/refs/heads/main/security/powershop-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Energy
- Australia
- Utilities
- Electricity
- Gas
- Consumer Data Right
- Energy Retail
- Smart Metering
- Solar
- Tariffs
- Open Data
---
