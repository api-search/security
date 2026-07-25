---
api_specs:
- filename: datastax-access-list-api-openapi.yml
  format: yaml
  label: DataStax Access List API
  slug: datastax-access-list-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datastax/refs/heads/main/openapi/datastax-access-list-api-openapi.yml
- filename: datastax-authentication-api-openapi.yml
  format: yaml
  label: DataStax Authentication API
  slug: datastax-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datastax/refs/heads/main/openapi/datastax-authentication-api-openapi.yml
- filename: datastax-clone-api-openapi.yml
  format: yaml
  label: DataStax Clone API
  slug: datastax-clone-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datastax/refs/heads/main/openapi/datastax-clone-api-openapi.yml
- filename: datastax-customer-keys-api-openapi.yml
  format: yaml
  label: DataStax Customer Keys API
  slug: datastax-customer-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datastax/refs/heads/main/openapi/datastax-customer-keys-api-openapi.yml
- filename: datastax-database-operations-api-openapi.yml
  format: yaml
  label: DataStax Database Operations API
  slug: datastax-database-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datastax/refs/heads/main/openapi/datastax-database-operations-api-openapi.yml
- filename: datastax-devops-access-list-api-openapi.yml
  format: yaml
  label: DataStax DevOps Access List API
  slug: datastax-devops-access-list-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datastax/refs/heads/main/openapi/datastax-devops-access-list-api-openapi.yml
- filename: datastax-enterprise-operations-api-openapi.yml
  format: yaml
  label: DataStax Enterprise Operations API
  slug: datastax-enterprise-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datastax/refs/heads/main/openapi/datastax-enterprise-operations-api-openapi.yml
- filename: datastax-migrations-api-openapi.yml
  format: yaml
  label: DataStax Migrations API
  slug: datastax-migrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datastax/refs/heads/main/openapi/datastax-migrations-api-openapi.yml
- filename: datastax-organization-operations-api-openapi.yml
  format: yaml
  label: DataStax Organization Operations API
  slug: datastax-organization-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datastax/refs/heads/main/openapi/datastax-organization-operations-api-openapi.yml
- filename: datastax-pcu-api-openapi.yml
  format: yaml
  label: DataStax PCU API
  slug: datastax-pcu-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datastax/refs/heads/main/openapi/datastax-pcu-api-openapi.yml
- filename: datastax-private-link-api-openapi.yml
  format: yaml
  label: DataStax Private Link API
  slug: datastax-private-link-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datastax/refs/heads/main/openapi/datastax-private-link-api-openapi.yml
- filename: datastax-regions-api-openapi.yml
  format: yaml
  label: DataStax Regions API
  slug: datastax-regions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datastax/refs/heads/main/openapi/datastax-regions-api-openapi.yml
- filename: datastax-roles-api-openapi.yml
  format: yaml
  label: DataStax Roles API
  slug: datastax-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datastax/refs/heads/main/openapi/datastax-roles-api-openapi.yml
- filename: datastax-scim-api-openapi.yml
  format: yaml
  label: DataStax SCIM API
  slug: datastax-scim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datastax/refs/heads/main/openapi/datastax-scim-api-openapi.yml
- filename: datastax-token-api-openapi.yml
  format: yaml
  label: DataStax Token API
  slug: datastax-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datastax/refs/heads/main/openapi/datastax-token-api-openapi.yml
- filename: datastax-users-api-openapi.yml
  format: yaml
  label: DataStax Users API
  slug: datastax-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datastax/refs/heads/main/openapi/datastax-users-api-openapi.yml
- filename: datastax-vpc-peering-api-openapi.yml
  format: yaml
  label: DataStax VPC Peering API
  slug: datastax-vpc-peering-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datastax/refs/heads/main/openapi/datastax-vpc-peering-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: datastax.com
  spf: true
hosts:
- cert_expires: Aug 26 15:21:08 2026 GMT
  host: www.datastax.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  7 23:59:59 2027 GMT
  host: docs.datastax.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 19 23:59:59 2027 GMT
  host: api.astra.datastax.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Datastax Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DataStax, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: DataStax
provider_slug: datastax
slug: datastax-domain-security
source_filename: datastax-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.datastax.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 15:21:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.datastax.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  7 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.astra.datastax.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: datastax.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datastax/refs/heads/main/security/datastax-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Enterprise
- Database
- Vector Database
- Cassandra
- Artificial Intelligence
- RAG
- Serverless
- Streaming
- Developer Tools
---
