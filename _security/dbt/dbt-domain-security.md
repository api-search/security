---
api_specs:
- filename: dbt-accounts-api-openapi.yml
  format: yaml
  label: dbt Accounts API
  slug: dbt-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dbt/openapi/dbt-accounts-api-openapi.yml
- filename: dbt-environments-api-openapi.yml
  format: yaml
  label: dbt Environments API
  slug: dbt-environments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dbt/openapi/dbt-environments-api-openapi.yml
- filename: dbt-jobs-api-openapi.yml
  format: yaml
  label: dbt Jobs API
  slug: dbt-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dbt/openapi/dbt-jobs-api-openapi.yml
- filename: dbt-metrics-api-openapi.yml
  format: yaml
  label: dbt Metrics API
  slug: dbt-metrics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dbt/openapi/dbt-metrics-api-openapi.yml
- filename: dbt-projects-api-openapi.yml
  format: yaml
  label: dbt Projects API
  slug: dbt-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dbt/openapi/dbt-projects-api-openapi.yml
- filename: dbt-runs-api-openapi.yml
  format: yaml
  label: dbt Runs API
  slug: dbt-runs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dbt/openapi/dbt-runs-api-openapi.yml
- filename: dbt-fastapi-api-openapi.yml
  format: yaml
  label: dbt Fast API
  slug: dbt-fastapi-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dbt/openapi/dbt-fastapi-api-openapi.yml
- filename: dbt-private-api-openapi.yml
  format: yaml
  label: dbt Private API
  slug: dbt-private-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dbt/openapi/dbt-private-api-openapi.yml
- filename: dbt-ready-api-openapi.yml
  format: yaml
  label: dbt Ready API
  slug: dbt-ready-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dbt/openapi/dbt-ready-api-openapi.yml
- filename: dbt-graph-ql-api-openapi.yml
  format: yaml
  label: dbt Graph QL API
  slug: dbt-graph-ql-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dbt/openapi/dbt-graph-ql-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: getdbt.com
  spf: true
hosts:
- cert_expires: Sep 20 08:58:58 2026 GMT
  host: www.getdbt.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 19:37:10 2026 GMT
  host: docs.getdbt.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 05:21:45 2026 GMT
  host: cloud.getdbt.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Dbt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for dbt, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: dbt
provider_slug: dbt
slug: dbt-domain-security
source_filename: dbt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getdbt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 08:58:58 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.getdbt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 19:37:10 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: cloud.getdbt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 05:21:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: getdbt.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/dbt/security/dbt-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Analytics Engineering
- Data
- ELT
- Metrics
- Project
- SQL
- Transformation
---
