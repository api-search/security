---
api_specs:
- filename: google-bigquery-analyticshub-organizations-api-openapi.yml
  format: yaml
  label: Google BigQuery Bigquery Analyticshub Organizations API
  slug: google-bigquery-analyticshub-organizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-bigquery/openapi/google-bigquery-analyticshub-organizations-api-openapi.yml
- filename: google-bigquery-analyticshub-projects-api-openapi.yml
  format: yaml
  label: Google BigQuery Bigquery Analyticshub Projects API
  slug: google-bigquery-analyticshub-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-bigquery/openapi/google-bigquery-analyticshub-projects-api-openapi.yml
- filename: google-bigquery-bigquery-datasets-api-openapi.yml
  format: yaml
  label: Google BigQuery Bigquery Bigquery Datasets API
  slug: google-bigquery-bigquery-datasets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-bigquery/openapi/google-bigquery-bigquery-datasets-api-openapi.yml
- filename: google-bigquery-bigquery-jobs-api-openapi.yml
  format: yaml
  label: Google BigQuery Bigquery Bigquery Jobs API
  slug: google-bigquery-bigquery-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-bigquery/openapi/google-bigquery-bigquery-jobs-api-openapi.yml
- filename: google-bigquery-bigquery-models-api-openapi.yml
  format: yaml
  label: Google BigQuery Bigquery Bigquery Models API
  slug: google-bigquery-bigquery-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-bigquery/openapi/google-bigquery-bigquery-models-api-openapi.yml
- filename: google-bigquery-bigquery-projects-api-openapi.yml
  format: yaml
  label: Google BigQuery Bigquery Bigquery Projects API
  slug: google-bigquery-bigquery-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-bigquery/openapi/google-bigquery-bigquery-projects-api-openapi.yml
- filename: google-bigquery-bigquery-routines-api-openapi.yml
  format: yaml
  label: Google BigQuery Bigquery Bigquery Routines API
  slug: google-bigquery-bigquery-routines-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-bigquery/openapi/google-bigquery-bigquery-routines-api-openapi.yml
- filename: google-bigquery-bigquery-row-access-policies-api-openapi.yml
  format: yaml
  label: Google BigQuery Bigquery Bigquery Row Access Policies API
  slug: google-bigquery-bigquery-row-access-policies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-bigquery/openapi/google-bigquery-bigquery-row-access-policies-api-openapi.yml
- filename: google-bigquery-bigquery-tabledata-api-openapi.yml
  format: yaml
  label: Google BigQuery Bigquery Bigquery Tabledata API
  slug: google-bigquery-bigquery-tabledata-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-bigquery/openapi/google-bigquery-bigquery-tabledata-api-openapi.yml
- filename: google-bigquery-bigquery-tables-api-openapi.yml
  format: yaml
  label: Google BigQuery Bigquery Bigquery Tables API
  slug: google-bigquery-bigquery-tables-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-bigquery/openapi/google-bigquery-bigquery-tables-api-openapi.yml
- filename: google-bigquery-bigqueryconnection-projects-api-openapi.yml
  format: yaml
  label: Google BigQuery Bigquery Bigqueryconnection Projects API
  slug: google-bigquery-bigqueryconnection-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-bigquery/openapi/google-bigquery-bigqueryconnection-projects-api-openapi.yml
- filename: google-bigquery-bigquerydatapolicy-projects-api-openapi.yml
  format: yaml
  label: Google BigQuery Bigquery Bigquerydatapolicy Projects API
  slug: google-bigquery-bigquerydatapolicy-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-bigquery/openapi/google-bigquery-bigquerydatapolicy-projects-api-openapi.yml
- filename: google-bigquery-bigquerydatatransfer-projects-api-openapi.yml
  format: yaml
  label: Google BigQuery Bigquery Bigquerydatatransfer Projects API
  slug: google-bigquery-bigquerydatatransfer-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-bigquery/openapi/google-bigquery-bigquerydatatransfer-projects-api-openapi.yml
- filename: google-bigquery-bigqueryreservation-projects-api-openapi.yml
  format: yaml
  label: Google BigQuery Bigquery Bigqueryreservation Projects API
  slug: google-bigquery-bigqueryreservation-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-bigquery/openapi/google-bigquery-bigqueryreservation-projects-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: google.com
  spf: true
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: googleapis.com
  spf: true
hosts:
- cert_expires: Dec 30 19:09:53 2026 GMT
  host: www.google.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 30 19:07:41 2026 GMT
  host: cloud.google.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 30 19:09:10 2026 GMT
  host: bigqueryconnection.googleapis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Google BigQuery Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Google BigQuery, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Google BigQuery
provider_slug: google-bigquery
slug: google-bigquery-domain-security
source_filename: google-bigquery-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 19:09:53 2026 GMT\n  hsts: false\n- host: cloud.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 19:07:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: bigqueryconnection.googleapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 19:09:10 2026 GMT\n  hsts: null\ndomains:\n- domain: google.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: googleapis.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/google-bigquery/security/google-bigquery-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Analytics
- Big Data
- Cloud
- Data Warehouse
- Serverless
- SQL
---
