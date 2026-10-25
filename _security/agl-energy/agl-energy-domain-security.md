---
api_specs:
- filename: agl-energy-data-holder-customers-api-openapi.yml
  format: yaml
  label: AGL Energy Data Holder Customers API
  slug: agl-energy-data-holder-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agl-energy/refs/heads/main/openapi/agl-energy-data-holder-customers-api-openapi.yml
- filename: agl-energy-data-holder-operations-api-openapi.yml
  format: yaml
  label: AGL Energy Data Holder Operations API
  slug: agl-energy-data-holder-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agl-energy/refs/heads/main/openapi/agl-energy-data-holder-operations-api-openapi.yml
- filename: agl-energy-distributed-energy-resources-api-openapi.yml
  format: yaml
  label: AGL Energy Distributed Energy Resources API
  slug: agl-energy-distributed-energy-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agl-energy/refs/heads/main/openapi/agl-energy-distributed-energy-resources-api-openapi.yml
- filename: agl-energy-electricity-service-points-api-openapi.yml
  format: yaml
  label: AGL Energy Electricity Service Points API
  slug: agl-energy-electricity-service-points-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agl-energy/refs/heads/main/openapi/agl-energy-electricity-service-points-api-openapi.yml
- filename: agl-energy-electricity-usage-api-openapi.yml
  format: yaml
  label: AGL Energy Electricity Usage API
  slug: agl-energy-electricity-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agl-energy/refs/heads/main/openapi/agl-energy-electricity-usage-api-openapi.yml
- filename: agl-energy-energy-account-balances-api-openapi.yml
  format: yaml
  label: AGL Energy Account Balances API
  slug: agl-energy-energy-account-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agl-energy/refs/heads/main/openapi/agl-energy-energy-account-balances-api-openapi.yml
- filename: agl-energy-energy-account-billing-api-openapi.yml
  format: yaml
  label: AGL Energy Account Billing API
  slug: agl-energy-energy-account-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agl-energy/refs/heads/main/openapi/agl-energy-energy-account-billing-api-openapi.yml
- filename: agl-energy-energy-accounts-api-openapi.yml
  format: yaml
  label: AGL Energy Accounts API
  slug: agl-energy-energy-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agl-energy/refs/heads/main/openapi/agl-energy-energy-accounts-api-openapi.yml
- filename: agl-energy-energy-plans-api-openapi.yml
  format: yaml
  label: AGL Energy Plans API
  slug: agl-energy-energy-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agl-energy/refs/heads/main/openapi/agl-energy-energy-plans-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "pki.goog"
  - 0 issue "amazontrust.com"
  - 0 issue "digicert.com"
  - 0 issue "amazonaws.com"
  - 0 issue "awstrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: agl.com.au
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
- cert_expires: Mar 25 23:59:59 2027 GMT
  host: www.agl.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  6 23:59:59 2026 GMT
  host: public.cdr.agl.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 31 23:59:59 2027 GMT
  host: cdr.energymadeeasy.gov.au
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Agl Energy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AGL Energy, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AGL Energy
provider_slug: agl-energy
slug: agl-energy-domain-security
source_filename: agl-energy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.agl.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 25 23:59:59 2027 GMT\n  hsts: null\n- host: public.cdr.agl.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 23:59:59 2026 GMT\n  hsts: null\n- host: cdr.energymadeeasy.gov.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: agl.com.au\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: energymadeeasy.gov.au\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc:\
  \ true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agl-energy/refs/heads/main/security/agl-energy-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Energy
- Australia
- Utilities
- Electricity
- Gas
- Energy Retailer
- Consumer Data Right
- CDR
- Smart Metering
- Solar
- DER
- Renewables
- Energy Markets
---
