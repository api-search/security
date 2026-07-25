---
api_specs:
- filename: dynamodb-streams-asyncapi.yml
  format: yaml
  label: Amazon DynamoDB Streams API
  slug: amazon-dynamodb-streams-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynamodb/refs/heads/main/asyncapi/dynamodb-streams-asyncapi.yml
- filename: dynamodb-backups-api-openapi.yml
  format: yaml
  label: Amazon DynamoDB Backups API
  slug: dynamodb-backups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynamodb/refs/heads/main/openapi/dynamodb-backups-api-openapi.yml
- filename: dynamodb-batch-operations-api-openapi.yml
  format: yaml
  label: Amazon DynamoDB Batch Operations API
  slug: dynamodb-batch-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynamodb/refs/heads/main/openapi/dynamodb-batch-operations-api-openapi.yml
- filename: dynamodb-exports-api-openapi.yml
  format: yaml
  label: Amazon DynamoDB Exports API
  slug: dynamodb-exports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynamodb/refs/heads/main/openapi/dynamodb-exports-api-openapi.yml
- filename: dynamodb-imports-api-openapi.yml
  format: yaml
  label: Amazon DynamoDB Imports API
  slug: dynamodb-imports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynamodb/refs/heads/main/openapi/dynamodb-imports-api-openapi.yml
- filename: dynamodb-items-api-openapi.yml
  format: yaml
  label: Amazon DynamoDB Items API
  slug: dynamodb-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynamodb/refs/heads/main/openapi/dynamodb-items-api-openapi.yml
- filename: dynamodb-listtagsofresource-api-openapi.yml
  format: yaml
  label: 'Amazon DynamoDB #ListTagsOfResource API'
  slug: dynamodb-listtagsofresource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynamodb/refs/heads/main/openapi/dynamodb-listtagsofresource-api-openapi.yml
- filename: dynamodb-partiql-api-openapi.yml
  format: yaml
  label: Amazon DynamoDB PartiQL API
  slug: dynamodb-partiql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynamodb/refs/heads/main/openapi/dynamodb-partiql-api-openapi.yml
- filename: dynamodb-queries-api-openapi.yml
  format: yaml
  label: Amazon DynamoDB Queries API
  slug: dynamodb-queries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynamodb/refs/heads/main/openapi/dynamodb-queries-api-openapi.yml
- filename: dynamodb-tables-api-openapi.yml
  format: yaml
  label: Amazon DynamoDB Tables API
  slug: dynamodb-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynamodb/refs/heads/main/openapi/dynamodb-tables-api-openapi.yml
- filename: dynamodb-tagresource-api-openapi.yml
  format: yaml
  label: 'Amazon DynamoDB #TagResource API'
  slug: dynamodb-tagresource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynamodb/refs/heads/main/openapi/dynamodb-tagresource-api-openapi.yml
- filename: dynamodb-transactions-api-openapi.yml
  format: yaml
  label: Amazon DynamoDB Transactions API
  slug: dynamodb-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynamodb/refs/heads/main/openapi/dynamodb-transactions-api-openapi.yml
- filename: dynamodb-ttl-api-openapi.yml
  format: yaml
  label: Amazon DynamoDB TTL API
  slug: dynamodb-ttl-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynamodb/refs/heads/main/openapi/dynamodb-ttl-api-openapi.yml
- filename: dynamodb-untagresource-api-openapi.yml
  format: yaml
  label: 'Amazon DynamoDB #UntagResource API'
  slug: dynamodb-untagresource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynamodb/refs/heads/main/openapi/dynamodb-untagresource-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amazon.com
  spf: true
hosts:
- cert_expires: Oct 17 23:59:59 2026 GMT
  host: aws.amazon.com
  hsts: true
  hsts_max_age: 47304000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  8 23:59:59 2026 GMT
  host: docs.aws.amazon.com
  hsts: true
  hsts_max_age: 47304000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dynamodb Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon DynamoDB, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amazon DynamoDB
provider_slug: dynamodb
slug: dynamodb-domain-security
source_filename: dynamodb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: docs.aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dynamodb/refs/heads/main/security/dynamodb-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud
- Database
- Document Store
- Key-Value
- Managed Service
- NoSQL
- Serverless
---
