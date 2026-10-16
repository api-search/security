---
api_specs:
- filename: dbt-se-agents-api-openapi.yml
  format: yaml
  label: DBT Capital Agents API
  slug: dbt-se-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dbt-se/refs/heads/main/openapi/dbt-se-agents-api-openapi.yml
- filename: dbt-se-banking-api-openapi.yml
  format: yaml
  label: DBT Capital Banking API
  slug: dbt-se-banking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dbt-se/refs/heads/main/openapi/dbt-se-banking-api-openapi.yml
- filename: dbt-se-bookkeeping-api-openapi.yml
  format: yaml
  label: DBT Capital Bookkeeping API
  slug: dbt-se-bookkeeping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dbt-se/refs/heads/main/openapi/dbt-se-bookkeeping-api-openapi.yml
- filename: dbt-se-documents-api-openapi.yml
  format: yaml
  label: DBT Capital Documents API
  slug: dbt-se-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dbt-se/refs/heads/main/openapi/dbt-se-documents-api-openapi.yml
- filename: dbt-se-files-api-openapi.yml
  format: yaml
  label: DBT Capital Files API
  slug: dbt-se-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dbt-se/refs/heads/main/openapi/dbt-se-files-api-openapi.yml
- filename: dbt-se-identity-api-openapi.yml
  format: yaml
  label: DBT Capital Identity API
  slug: dbt-se-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dbt-se/refs/heads/main/openapi/dbt-se-identity-api-openapi.yml
- filename: dbt-se-llm-api-openapi.yml
  format: yaml
  label: DBT Capital LLM API
  slug: dbt-se-llm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dbt-se/refs/heads/main/openapi/dbt-se-llm-api-openapi.yml
- filename: dbt-se-notification-api-openapi.yml
  format: yaml
  label: DBT Capital Notification API
  slug: dbt-se-notification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dbt-se/refs/heads/main/openapi/dbt-se-notification-api-openapi.yml
- filename: dbt-se-portfolio-api-openapi.yml
  format: yaml
  label: DBT Capital Portfolio API
  slug: dbt-se-portfolio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dbt-se/refs/heads/main/openapi/dbt-se-portfolio-api-openapi.yml
- filename: dbt-se-prospect-api-openapi.yml
  format: yaml
  label: DBT Capital Prospect API
  slug: dbt-se-prospect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dbt-se/refs/heads/main/openapi/dbt-se-prospect-api-openapi.yml
- filename: dbt-se-regulatory-records-api-openapi.yml
  format: yaml
  label: DBT Capital Regulatory Records API
  slug: dbt-se-regulatory-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dbt-se/refs/heads/main/openapi/dbt-se-regulatory-records-api-openapi.yml
- filename: dbt-se-uc-api-openapi.yml
  format: yaml
  label: DBT Capital UC API
  slug: dbt-se-uc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dbt-se/refs/heads/main/openapi/dbt-se-uc-api-openapi.yml
- filename: dbt-se-upload-api-openapi.yml
  format: yaml
  label: DBT Capital Upload API
  slug: dbt-se-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dbt-se/refs/heads/main/openapi/dbt-se-upload-api-openapi.yml
- filename: dbt-se-workbooks-api-openapi.yml
  format: yaml
  label: DBT Capital Workbooks API
  slug: dbt-se-workbooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dbt-se/refs/heads/main/openapi/dbt-se-workbooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: dbt.se
  spf: true
hosts:
- cert_expires: Mar 18 23:59:59 2027 GMT
  host: dbt.se
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dbt Se Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DBT Capital, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: DBT Capital
provider_slug: dbt-se
slug: dbt-se-domain-security
source_filename: dbt-se-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dbt.se\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 18 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: dbt.se\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dbt-se/refs/heads/main/security/dbt-se-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Finance
- Loans
- Sweden
- Business
---
