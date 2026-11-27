---
api_specs:
- filename: google-cloud-sql-databases-api-openapi.yml
  format: yaml
  label: Google Cloud SQL Databases API
  slug: google-cloud-sql-databases-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-sql/openapi/google-cloud-sql-databases-api-openapi.yml
- filename: google-cloud-sql-instances-api-openapi.yml
  format: yaml
  label: Google Cloud SQL Instances API
  slug: google-cloud-sql-instances-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-sql/openapi/google-cloud-sql-instances-api-openapi.yml
- filename: google-cloud-sql-users-api-openapi.yml
  format: yaml
  label: Google Cloud SQL Users API
  slug: google-cloud-sql-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-sql/openapi/google-cloud-sql-users-api-openapi.yml
- filename: google-cloud-sql-backups-api-openapi.yml
  format: yaml
  label: Google Cloud SQL Cloud Sql Backups API
  slug: google-cloud-sql-backups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-sql/openapi/google-cloud-sql-backups-api-openapi.yml
- filename: google-cloud-sql-connect-api-openapi.yml
  format: yaml
  label: Google Cloud SQL Cloud Sql Connect API
  slug: google-cloud-sql-connect-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-sql/openapi/google-cloud-sql-connect-api-openapi.yml
- filename: google-cloud-sql-flags-api-openapi.yml
  format: yaml
  label: Google Cloud SQL Cloud Sql Flags API
  slug: google-cloud-sql-flags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-sql/openapi/google-cloud-sql-flags-api-openapi.yml
- filename: google-cloud-sql-operations-api-openapi.yml
  format: yaml
  label: Google Cloud SQL Cloud Sql Operations API
  slug: google-cloud-sql-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-sql/openapi/google-cloud-sql-operations-api-openapi.yml
- filename: google-cloud-sql-projects-api-openapi.yml
  format: yaml
  label: Google Cloud SQL Cloud Sql Projects API
  slug: google-cloud-sql-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-sql/openapi/google-cloud-sql-projects-api-openapi.yml
- filename: google-cloud-sql-tiers-api-openapi.yml
  format: yaml
  label: Google Cloud SQL Cloud Sql Tiers API
  slug: google-cloud-sql-tiers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-sql/openapi/google-cloud-sql-tiers-api-openapi.yml
- filename: google-cloud-sql-backupruns-api-openapi.yml
  format: yaml
  label: Google Cloud SQL Backup Runs API
  slug: google-cloud-sql-backupruns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-sql/openapi/google-cloud-sql-backupruns-api-openapi.yml
- filename: google-cloud-sql-bluegreendeployments-api-openapi.yml
  format: yaml
  label: Google Cloud SQL Blue Green Deployments API
  slug: google-cloud-sql-bluegreendeployments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-sql/openapi/google-cloud-sql-bluegreendeployments-api-openapi.yml
- filename: google-cloud-sql-sslcerts-api-openapi.yml
  format: yaml
  label: Google Cloud SQL Ssl Certs API
  slug: google-cloud-sql-sslcerts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-sql/openapi/google-cloud-sql-sslcerts-api-openapi.yml
- filename: google-cloud-sql-workloadcaptures-api-openapi.yml
  format: yaml
  label: Google Cloud SQL Workload Captures API
  slug: google-cloud-sql-workloadcaptures-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-sql/openapi/google-cloud-sql-workloadcaptures-api-openapi.yml
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
  host: sqladmin.googleapis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Google Cloud SQL Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Google Cloud SQL, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Google Cloud SQL
provider_slug: google-cloud-sql
slug: google-cloud-sql-domain-security
source_filename: google-cloud-sql-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 19:09:53 2026 GMT\n  hsts: false\n- host: cloud.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 19:07:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: sqladmin.googleapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 19:09:10 2026 GMT\n  hsts: null\ndomains:\n- domain: google.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: googleapis.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/google-cloud-sql/security/google-cloud-sql-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Database
- Google Cloud
- MySQL
- PostgreSQL
- Relational
- SQL
---
