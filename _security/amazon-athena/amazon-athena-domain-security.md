---
api_specs:
- filename: amazon-athena-data-catalogs-api-openapi.yml
  format: yaml
  label: Amazon Athena Data Catalogs API
  slug: amazon-athena-data-catalogs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-athena/openapi/amazon-athena-data-catalogs-api-openapi.yml
- filename: amazon-athena-databases-api-openapi.yml
  format: yaml
  label: Amazon Athena Databases API
  slug: amazon-athena-databases-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-athena/openapi/amazon-athena-databases-api-openapi.yml
- filename: amazon-athena-named-queries-api-openapi.yml
  format: yaml
  label: Amazon Athena Named Queries API
  slug: amazon-athena-named-queries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-athena/openapi/amazon-athena-named-queries-api-openapi.yml
- filename: amazon-athena-prepared-statements-api-openapi.yml
  format: yaml
  label: Amazon Athena Prepared Statements API
  slug: amazon-athena-prepared-statements-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-athena/openapi/amazon-athena-prepared-statements-api-openapi.yml
- filename: amazon-athena-query-executions-api-openapi.yml
  format: yaml
  label: Amazon Athena Query Executions API
  slug: amazon-athena-query-executions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-athena/openapi/amazon-athena-query-executions-api-openapi.yml
- filename: amazon-athena-table-metadata-api-openapi.yml
  format: yaml
  label: Amazon Athena Table Metadata API
  slug: amazon-athena-table-metadata-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-athena/openapi/amazon-athena-table-metadata-api-openapi.yml
- filename: amazon-athena-tags-api-openapi.yml
  format: yaml
  label: Amazon Athena Tags API
  slug: amazon-athena-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-athena/openapi/amazon-athena-tags-api-openapi.yml
- filename: amazon-athena-work-groups-api-openapi.yml
  format: yaml
  label: Amazon Athena Work Groups API
  slug: amazon-athena-work-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-athena/openapi/amazon-athena-work-groups-api-openapi.yml
- filename: amazon-athena-calculation-execution-api-openapi.yml
  format: yaml
  label: Amazon Athena Athena Calculation Execution API
  slug: amazon-athena-calculation-execution-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-athena/openapi/amazon-athena-calculation-execution-api-openapi.yml
- filename: amazon-athena-capacity-reservation-api-openapi.yml
  format: yaml
  label: Amazon Athena Athena Capacity Reservation API
  slug: amazon-athena-capacity-reservation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-athena/openapi/amazon-athena-capacity-reservation-api-openapi.yml
- filename: amazon-athena-notebook-api-openapi.yml
  format: yaml
  label: Amazon Athena Athena Notebook API
  slug: amazon-athena-notebook-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-athena/openapi/amazon-athena-notebook-api-openapi.yml
- filename: amazon-athena-notebook-metadata-api-openapi.yml
  format: yaml
  label: Amazon Athena Athena Notebook Metadata API
  slug: amazon-athena-notebook-metadata-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-athena/openapi/amazon-athena-notebook-metadata-api-openapi.yml
- filename: amazon-athena-operations-api-openapi.yml
  format: yaml
  label: Amazon Athena Athena Operations API
  slug: amazon-athena-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-athena/openapi/amazon-athena-operations-api-openapi.yml
- filename: amazon-athena-session-api-openapi.yml
  format: yaml
  label: Amazon Athena Athena Session API
  slug: amazon-athena-session-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-athena/openapi/amazon-athena-session-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amazon.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amazonaws.com
  spf: true
hosts:
- cert_expires: Dec  8 23:59:59 2026 GMT
  host: docs.aws.amazon.com
  hsts: true
  hsts_max_age: 47304000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  8 23:59:59 2026 GMT
  host: athena.us-east-1.amazonaws.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Amazon Athena Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon Athena, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amazon Athena
provider_slug: amazon-athena
slug: amazon-athena-domain-security
source_filename: amazon-athena-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: athena.us-east-1.amazonaws.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: amazonaws.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/amazon-athena/security/amazon-athena-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Amazon Athena
- SQL
- Analytics
- Serverless
---
