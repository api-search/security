---
api_specs:
- filename: dynamodb-openapi.yml
  format: yaml
  label: Amazon DynamoDB API
  slug: amazon-dynamodb-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynamodb/refs/heads/main/openapi/dynamodb-openapi.yml
- filename: dynamodb-streams-asyncapi.yml
  format: yaml
  label: Amazon DynamoDB Streams API
  slug: amazon-dynamodb-streams-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynamodb/refs/heads/main/asyncapi/dynamodb-streams-asyncapi.yml
- filename: openapi.yaml
  format: yaml
  label: Amazon DynamoDB Accelerator (DAX) API
  slug: amazon-dynamodb-accelerator-dax-api
  spec_type: OpenAPI
  url: https://api.apis.guru/v2/specs/amazonaws.com/dax/2017-04-19/openapi.yaml
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
