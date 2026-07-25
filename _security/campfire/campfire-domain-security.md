---
api_specs:
- filename: campfire-accounts-payable-api-openapi.yml
  format: yaml
  label: Campfire Accounts Payable API
  slug: campfire-accounts-payable-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire/refs/heads/main/openapi/campfire-accounts-payable-api-openapi.yml
- filename: campfire-accounts-receivable-api-openapi.yml
  format: yaml
  label: Campfire Accounts Receivable API
  slug: campfire-accounts-receivable-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire/refs/heads/main/openapi/campfire-accounts-receivable-api-openapi.yml
- filename: campfire-bank-reconciliation-api-openapi.yml
  format: yaml
  label: Campfire Bank Reconciliation API
  slug: campfire-bank-reconciliation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire/refs/heads/main/openapi/campfire-bank-reconciliation-api-openapi.yml
- filename: campfire-cash-management-api-openapi.yml
  format: yaml
  label: Campfire Cash Management API
  slug: campfire-cash-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire/refs/heads/main/openapi/campfire-cash-management-api-openapi.yml
- filename: campfire-coa-api-openapi.yml
  format: yaml
  label: Campfire coa API
  slug: campfire-coa-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire/refs/heads/main/openapi/campfire-coa-api-openapi.yml
- filename: campfire-company-objects-api-openapi.yml
  format: yaml
  label: Campfire Company Objects API
  slug: campfire-company-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire/refs/heads/main/openapi/campfire-company-objects-api-openapi.yml
- filename: campfire-core-accounting-api-openapi.yml
  format: yaml
  label: Campfire Core Accounting API
  slug: campfire-core-accounting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire/refs/heads/main/openapi/campfire-core-accounting-api-openapi.yml
- filename: campfire-custom-fields-api-openapi.yml
  format: yaml
  label: Campfire Custom Fields API
  slug: campfire-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire/refs/heads/main/openapi/campfire-custom-fields-api-openapi.yml
- filename: campfire-financial-statements-api-openapi.yml
  format: yaml
  label: Campfire Financial Statements API
  slug: campfire-financial-statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire/refs/heads/main/openapi/campfire-financial-statements-api-openapi.yml
- filename: campfire-integrations-api-openapi.yml
  format: yaml
  label: Campfire Integrations API
  slug: campfire-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire/refs/heads/main/openapi/campfire-integrations-api-openapi.yml
- filename: campfire-revenue-recognition-api-openapi.yml
  format: yaml
  label: Campfire Revenue Recognition API
  slug: campfire-revenue-recognition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire/refs/heads/main/openapi/campfire-revenue-recognition-api-openapi.yml
- filename: campfire-settings-api-openapi.yml
  format: yaml
  label: Campfire Settings API
  slug: campfire-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire/refs/heads/main/openapi/campfire-settings-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: meetcampfire.com
  spf: true
hosts:
- cert_expires: Mar 12 23:59:59 2027 GMT
  host: api.meetcampfire.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Campfire Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Campfire, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Campfire
provider_slug: campfire
slug: campfire-domain-security
source_filename: campfire-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.meetcampfire.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 12 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: meetcampfire.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/campfire/refs/heads/main/security/campfire-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Accounting
- ERP
- Finance
- Revenue Recognition
- Accounts Payable
- Accounts Receivable
- AI
---
