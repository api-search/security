---
api_specs:
- filename: aer-data-holder-customers-api-openapi.yml
  format: yaml
  label: Australian Energy Regulator Data Holder Customers API
  slug: aer-data-holder-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aer/refs/heads/main/openapi/aer-data-holder-customers-api-openapi.yml
- filename: aer-data-holder-operations-api-openapi.yml
  format: yaml
  label: Australian Energy Regulator Data Holder Operations API
  slug: aer-data-holder-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aer/refs/heads/main/openapi/aer-data-holder-operations-api-openapi.yml
- filename: aer-distributed-energy-resources-api-openapi.yml
  format: yaml
  label: Australian Energy Regulator Distributed Energy Resources API
  slug: aer-distributed-energy-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aer/refs/heads/main/openapi/aer-distributed-energy-resources-api-openapi.yml
- filename: aer-electricity-service-points-api-openapi.yml
  format: yaml
  label: Australian Energy Regulator Electricity Service Points API
  slug: aer-electricity-service-points-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aer/refs/heads/main/openapi/aer-electricity-service-points-api-openapi.yml
- filename: aer-electricity-usage-api-openapi.yml
  format: yaml
  label: Australian Energy Regulator Electricity Usage API
  slug: aer-electricity-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aer/refs/heads/main/openapi/aer-electricity-usage-api-openapi.yml
- filename: aer-energy-account-balances-api-openapi.yml
  format: yaml
  label: Australian Energy Regulator Energy Account Balances API
  slug: aer-energy-account-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aer/refs/heads/main/openapi/aer-energy-account-balances-api-openapi.yml
- filename: aer-energy-account-billing-api-openapi.yml
  format: yaml
  label: Australian Energy Regulator Energy Account Billing API
  slug: aer-energy-account-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aer/refs/heads/main/openapi/aer-energy-account-billing-api-openapi.yml
- filename: aer-energy-accounts-api-openapi.yml
  format: yaml
  label: Australian Energy Regulator Energy Accounts API
  slug: aer-energy-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aer/refs/heads/main/openapi/aer-energy-accounts-api-openapi.yml
- filename: aer-energy-plans-api-openapi.yml
  format: yaml
  label: Australian Energy Regulator Energy Plans API
  slug: aer-energy-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aer/refs/heads/main/openapi/aer-energy-plans-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: aer.gov.au
  spf: true
- caa:
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "awstrust.com"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: energymadeeasy.gov.au
  spf: true
hosts:
- cert_expires: Oct  5 08:19:20 2026 GMT
  host: www.aer.gov.au
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 17 23:59:59 2027 GMT
  host: www.energymadeeasy.gov.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 31 23:59:59 2027 GMT
  host: cdr.energymadeeasy.gov.au
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Australian Energy Regulator, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Australian Energy Regulator
provider_slug: aer
slug: aer-domain-security
source_filename: aer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aer.gov.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 08:19:20 2026 GMT\n  hsts: null\n- host: www.energymadeeasy.gov.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: cdr.energymadeeasy.gov.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: aer.gov.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: energymadeeasy.gov.au\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aer/refs/heads/main/security/aer-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- Australia
- Utilities
- Electricity
- Gas
- Energy Markets
- Consumer Data Right
- Retail Energy
- Regulations
- Government
- Open Data
- Smart Metering
---
