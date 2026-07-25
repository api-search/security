---
api_specs:
- filename: ntropy-account-holder-api-openapi.yml
  format: yaml
  label: Ntropy Account Holder API
  slug: ntropy-account-holder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ntropy/refs/heads/main/openapi/ntropy-account-holder-api-openapi.yml
- filename: ntropy-accountholders-api-openapi.yml
  format: yaml
  label: Ntropy accountHolders API
  slug: ntropy-accountholders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ntropy/refs/heads/main/openapi/ntropy-accountholders-api-openapi.yml
- filename: ntropy-bank-statements-api-openapi.yml
  format: yaml
  label: Ntropy Bank statements API
  slug: ntropy-bank-statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ntropy/refs/heads/main/openapi/ntropy-bank-statements-api-openapi.yml
- filename: ntropy-bankstatements-api-openapi.yml
  format: yaml
  label: Ntropy bankStatements API
  slug: ntropy-bankstatements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ntropy/refs/heads/main/openapi/ntropy-bankstatements-api-openapi.yml
- filename: ntropy-batches-api-openapi.yml
  format: yaml
  label: Ntropy batches API
  slug: ntropy-batches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ntropy/refs/heads/main/openapi/ntropy-batches-api-openapi.yml
- filename: ntropy-categories-api-openapi.yml
  format: yaml
  label: Ntropy categories API
  slug: ntropy-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ntropy/refs/heads/main/openapi/ntropy-categories-api-openapi.yml
- filename: ntropy-enrichment-api-openapi.yml
  format: yaml
  label: Ntropy Enrichment API
  slug: ntropy-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ntropy/refs/heads/main/openapi/ntropy-enrichment-api-openapi.yml
- filename: ntropy-entities-api-openapi.yml
  format: yaml
  label: Ntropy entities API
  slug: ntropy-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ntropy/refs/heads/main/openapi/ntropy-entities-api-openapi.yml
- filename: ntropy-labels-api-openapi.yml
  format: yaml
  label: Ntropy Labels API
  slug: ntropy-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ntropy/refs/heads/main/openapi/ntropy-labels-api-openapi.yml
- filename: ntropy-misc-api-openapi.yml
  format: yaml
  label: Ntropy Misc API
  slug: ntropy-misc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ntropy/refs/heads/main/openapi/ntropy-misc-api-openapi.yml
- filename: ntropy-personalization-api-openapi.yml
  format: yaml
  label: Ntropy personalization API
  slug: ntropy-personalization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ntropy/refs/heads/main/openapi/ntropy-personalization-api-openapi.yml
- filename: ntropy-recurrence-api-openapi.yml
  format: yaml
  label: Ntropy recurrence API
  slug: ntropy-recurrence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ntropy/refs/heads/main/openapi/ntropy-recurrence-api-openapi.yml
- filename: ntropy-reporting-api-openapi.yml
  format: yaml
  label: Ntropy Reporting API
  slug: ntropy-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ntropy/refs/heads/main/openapi/ntropy-reporting-api-openapi.yml
- filename: ntropy-reports-api-openapi.yml
  format: yaml
  label: Ntropy reports API
  slug: ntropy-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ntropy/refs/heads/main/openapi/ntropy-reports-api-openapi.yml
- filename: ntropy-transactions-api-openapi.yml
  format: yaml
  label: Ntropy transactions API
  slug: ntropy-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ntropy/refs/heads/main/openapi/ntropy-transactions-api-openapi.yml
- filename: ntropy-webhooks-api-openapi.yml
  format: yaml
  label: Ntropy webhooks API
  slug: ntropy-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ntropy/refs/heads/main/openapi/ntropy-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ntropy.network
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ntropy.com
  spf: true
hosts:
- cert_expires: Aug 22 22:45:16 2026 GMT
  host: ntropy.network
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 14:59:23 2026 GMT
  host: api.ntropy.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ntropy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ntropy, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ntropy
provider_slug: ntropy
slug: ntropy-domain-security
source_filename: ntropy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ntropy.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 22:45:16 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.ntropy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 14:59:23 2026 GMT\n  hsts: null\ndomains:\n- domain: ntropy.network\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: ntropy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ntropy/refs/heads/main/security/ntropy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Transaction Enrichment
- Financial Data
- Data Enrichment
- Bank Statements
- Categorization
- Underwriting
---
