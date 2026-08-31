---
api_specs:
- filename: alinta-energy-data-holder-customers-api-openapi.yml
  format: yaml
  label: Alinta Energy Data Holder Customers API
  slug: alinta-energy-data-holder-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alinta-energy/refs/heads/main/openapi/alinta-energy-data-holder-customers-api-openapi.yml
- filename: alinta-energy-data-holder-operations-api-openapi.yml
  format: yaml
  label: Alinta Energy Data Holder Operations API
  slug: alinta-energy-data-holder-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alinta-energy/refs/heads/main/openapi/alinta-energy-data-holder-operations-api-openapi.yml
- filename: alinta-energy-distributed-energy-resources-api-openapi.yml
  format: yaml
  label: Alinta Energy Distributed Energy Resources API
  slug: alinta-energy-distributed-energy-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alinta-energy/refs/heads/main/openapi/alinta-energy-distributed-energy-resources-api-openapi.yml
- filename: alinta-energy-electricity-service-points-api-openapi.yml
  format: yaml
  label: Alinta Energy Electricity Service Points API
  slug: alinta-energy-electricity-service-points-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alinta-energy/refs/heads/main/openapi/alinta-energy-electricity-service-points-api-openapi.yml
- filename: alinta-energy-electricity-usage-api-openapi.yml
  format: yaml
  label: Alinta Energy Electricity Usage API
  slug: alinta-energy-electricity-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alinta-energy/refs/heads/main/openapi/alinta-energy-electricity-usage-api-openapi.yml
- filename: alinta-energy-energy-account-balances-api-openapi.yml
  format: yaml
  label: Alinta Energy Energy Account Balances API
  slug: alinta-energy-energy-account-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alinta-energy/refs/heads/main/openapi/alinta-energy-energy-account-balances-api-openapi.yml
- filename: alinta-energy-energy-account-billing-api-openapi.yml
  format: yaml
  label: Alinta Energy Energy Account Billing API
  slug: alinta-energy-energy-account-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alinta-energy/refs/heads/main/openapi/alinta-energy-energy-account-billing-api-openapi.yml
- filename: alinta-energy-energy-accounts-api-openapi.yml
  format: yaml
  label: Alinta Energy Energy Accounts API
  slug: alinta-energy-energy-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alinta-energy/refs/heads/main/openapi/alinta-energy-energy-accounts-api-openapi.yml
- filename: alinta-energy-energy-plans-api-openapi.yml
  format: yaml
  label: Alinta Energy Energy Plans API
  slug: alinta-energy-energy-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alinta-energy/refs/heads/main/openapi/alinta-energy-energy-plans-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: alintaenergy.com.au
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
- cert_expires: Aug 26 05:20:32 2026 GMT
  host: www.alintaenergy.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 24 23:59:59 2026 GMT
  host: public.cdr.alintaenergy.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 17 23:59:59 2027 GMT
  host: www.energymadeeasy.gov.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Alinta Energy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alinta Energy, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Alinta Energy
provider_slug: alinta-energy
slug: alinta-energy-domain-security
source_filename: alinta-energy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.alintaenergy.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 05:20:32 2026 GMT\n  hsts: null\n- host: public.cdr.alintaenergy.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 23:59:59 2026 GMT\n  hsts: null\n- host: www.energymadeeasy.gov.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: alintaenergy.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: energymadeeasy.gov.au\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alinta-energy/refs/heads/main/security/alinta-energy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- Australia
- Utilities
- Electricity
- Gas
- Energy Retail
- Consumer Data Right
- CDR
- Open Energy Data
- Smart Metering
- Renewables
- Generation
---
