---
api_specs:
- filename: red-energy-data-holder-customers-api-openapi.yml
  format: yaml
  label: Red Energy Data Holder Customers API
  slug: red-energy-data-holder-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-energy/refs/heads/main/openapi/red-energy-data-holder-customers-api-openapi.yml
- filename: red-energy-data-holder-operations-api-openapi.yml
  format: yaml
  label: Red Energy Data Holder Operations API
  slug: red-energy-data-holder-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-energy/refs/heads/main/openapi/red-energy-data-holder-operations-api-openapi.yml
- filename: red-energy-distributed-energy-resources-api-openapi.yml
  format: yaml
  label: Red Energy Distributed Energy Resources API
  slug: red-energy-distributed-energy-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-energy/refs/heads/main/openapi/red-energy-distributed-energy-resources-api-openapi.yml
- filename: red-energy-electricity-service-points-api-openapi.yml
  format: yaml
  label: Red Energy Electricity Service Points API
  slug: red-energy-electricity-service-points-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-energy/refs/heads/main/openapi/red-energy-electricity-service-points-api-openapi.yml
- filename: red-energy-electricity-usage-api-openapi.yml
  format: yaml
  label: Red Energy Electricity Usage API
  slug: red-energy-electricity-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-energy/refs/heads/main/openapi/red-energy-electricity-usage-api-openapi.yml
- filename: red-energy-energy-account-balances-api-openapi.yml
  format: yaml
  label: Red Energy Account Balances API
  slug: red-energy-energy-account-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-energy/refs/heads/main/openapi/red-energy-energy-account-balances-api-openapi.yml
- filename: red-energy-energy-account-billing-api-openapi.yml
  format: yaml
  label: Red Energy Account Billing API
  slug: red-energy-energy-account-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-energy/refs/heads/main/openapi/red-energy-energy-account-billing-api-openapi.yml
- filename: red-energy-energy-accounts-api-openapi.yml
  format: yaml
  label: Red Energy Accounts API
  slug: red-energy-energy-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-energy/refs/heads/main/openapi/red-energy-energy-accounts-api-openapi.yml
- filename: red-energy-energy-plans-api-openapi.yml
  format: yaml
  label: Red Energy Plans API
  slug: red-energy-energy-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-energy/refs/heads/main/openapi/red-energy-energy-plans-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: redenergy.com.au
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
- cert_expires: Dec 10 04:13:26 2026 GMT
  host: www.redenergy.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 31 23:59:59 2027 GMT
  host: cdr.energymadeeasy.gov.au
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Red Energy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Red Energy, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Red Energy
provider_slug: red-energy
slug: red-energy-domain-security
source_filename: red-energy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.redenergy.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 04:13:26 2026 GMT\n  hsts: null\n- host: cdr.energymadeeasy.gov.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: redenergy.com.au\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: energymadeeasy.gov.au\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/red-energy/refs/heads/main/security/red-energy-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Energy
- Australia
- Utilities
- Electricity
- Gas
- Energy Retail
- Consumer Data Right
- CDR
- Product Reference Data
- Smart Metering
- Open Data
---
