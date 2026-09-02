---
api_specs:
- filename: oracle-platforms-analytics-api-openapi.yml
  format: yaml
  label: Oracle Platforms Analytics API
  slug: oracle-platforms-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-platforms/refs/heads/main/openapi/oracle-platforms-analytics-api-openapi.yml
- filename: oracle-platforms-blockstorage-api-openapi.yml
  format: yaml
  label: Oracle Platforms Blockstorage API
  slug: oracle-platforms-blockstorage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-platforms/refs/heads/main/openapi/oracle-platforms-blockstorage-api-openapi.yml
- filename: oracle-platforms-compute-api-openapi.yml
  format: yaml
  label: Oracle Platforms Compute API
  slug: oracle-platforms-compute-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-platforms/refs/heads/main/openapi/oracle-platforms-compute-api-openapi.yml
- filename: oracle-platforms-computemanagement-api-openapi.yml
  format: yaml
  label: Oracle Platforms Compute Management API
  slug: oracle-platforms-computemanagement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-platforms/refs/heads/main/openapi/oracle-platforms-computemanagement-api-openapi.yml
- filename: oracle-platforms-database-api-openapi.yml
  format: yaml
  label: Oracle Platforms Database API
  slug: oracle-platforms-database-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-platforms/refs/heads/main/openapi/oracle-platforms-database-api-openapi.yml
- filename: oracle-platforms-datascience-api-openapi.yml
  format: yaml
  label: Oracle Platforms Data Science API
  slug: oracle-platforms-datascience-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-platforms/refs/heads/main/openapi/oracle-platforms-datascience-api-openapi.yml
- filename: oracle-platforms-integrationinstance-api-openapi.yml
  format: yaml
  label: Oracle Platforms Integration Instance API
  slug: oracle-platforms-integrationinstance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-platforms/refs/heads/main/openapi/oracle-platforms-integrationinstance-api-openapi.yml
- filename: oracle-platforms-oceinstance-api-openapi.yml
  format: yaml
  label: Oracle Platforms Oce Instance API
  slug: oracle-platforms-oceinstance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-platforms/refs/heads/main/openapi/oracle-platforms-oceinstance-api-openapi.yml
- filename: oracle-platforms-virtualnetwork-api-openapi.yml
  format: yaml
  label: Oracle Platforms Virtual Network API
  slug: oracle-platforms-virtualnetwork-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-platforms/refs/heads/main/openapi/oracle-platforms-virtualnetwork-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: oracle.com
  spf: true
- caa:
  - 0 issue "digicert.com"
  - 0 issue "symantec.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: oraclecloud.com
  spf: true
hosts:
- cert_expires: Nov 15 23:59:59 2026 GMT
  host: docs.oracle.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: integration.ocp.oraclecloud.com
  https: false
- cert_expires: Feb  6 23:59:59 2027 GMT
  host: www.oraclecloud.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Oracle Platforms Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Oracle Platforms, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Oracle Platforms
provider_slug: oracle-platforms
slug: oracle-platforms-domain-security
source_filename: oracle-platforms-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.oracle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 23:59:59 2026 GMT\n  hsts: false\n- host: integration.ocp.oraclecloud.com\n  https: false\n- host: www.oraclecloud.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  6 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: oracle.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: oraclecloud.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"symantec.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oracle-platforms/refs/heads/main/security/oracle-platforms-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Analytics
- Cloud Computing
- Database
- Enterprise Software
- Infrastructure-as-a-Service
- Integration
- Machine-Learning
- Platform-as-a-Service
- Software-as-a-Service
---
