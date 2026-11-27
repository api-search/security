---
api_specs:
- filename: kinesis-liststreams-api-openapi.yml
  format: yaml
  label: AWS Kinesis ListStreams API
  slug: kinesis-liststreams-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kinesis/openapi/kinesis-liststreams-api-openapi.yml
- filename: kinesis-amazon-kinesis-analytics-api-openapi.yml
  format: yaml
  label: AWS Kinesis Amazon Kinesis Analytics API
  slug: kinesis-amazon-kinesis-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kinesis/openapi/kinesis-amazon-kinesis-analytics-api-openapi.yml
- filename: kinesis-amazon-kinesis-api-openapi.yml
  format: yaml
  label: AWS Kinesis Amazon Kinesis API
  slug: kinesis-amazon-kinesis-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kinesis/openapi/kinesis-amazon-kinesis-api-openapi.yml
- filename: kinesis-amazon-kinesis-firehose-api-openapi.yml
  format: yaml
  label: AWS Kinesis Amazon Kinesis Firehose API
  slug: kinesis-amazon-kinesis-firehose-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kinesis/openapi/kinesis-amazon-kinesis-firehose-api-openapi.yml
- filename: kinesis-channel-api-openapi.yml
  format: yaml
  label: AWS Kinesis Channel API
  slug: kinesis-channel-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kinesis/openapi/kinesis-channel-api-openapi.yml
- filename: kinesis-operations-api-openapi.yml
  format: yaml
  label: AWS Kinesis Operations API
  slug: kinesis-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kinesis/openapi/kinesis-operations-api-openapi.yml
- filename: kinesis-resource-policy-api-openapi.yml
  format: yaml
  label: AWS Kinesis Resource Policy API
  slug: kinesis-resource-policy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kinesis/openapi/kinesis-resource-policy-api-openapi.yml
- filename: kinesis-create-stream-api-openapi.yml
  format: yaml
  label: AWS Kinesis Create Stream API
  slug: kinesis-create-stream-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kinesis/openapi/kinesis-create-stream-api-openapi.yml
- filename: kinesis-delete-stream-api-openapi.yml
  format: yaml
  label: AWS Kinesis Delete Stream API
  slug: kinesis-delete-stream-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kinesis/openapi/kinesis-delete-stream-api-openapi.yml
- filename: kinesis-describe-stream-api-openapi.yml
  format: yaml
  label: AWS Kinesis Describe Stream API
  slug: kinesis-describe-stream-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kinesis/openapi/kinesis-describe-stream-api-openapi.yml
- filename: kinesis-list-tags-for-resource-api-openapi.yml
  format: yaml
  label: AWS Kinesis List Tags For Resource API
  slug: kinesis-list-tags-for-resource-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kinesis/openapi/kinesis-list-tags-for-resource-api-openapi.yml
- filename: kinesis-list-tags-for-stream-api-openapi.yml
  format: yaml
  label: AWS Kinesis List Tags For Stream API
  slug: kinesis-list-tags-for-stream-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kinesis/openapi/kinesis-list-tags-for-stream-api-openapi.yml
- filename: kinesis-tag-resource-api-openapi.yml
  format: yaml
  label: AWS Kinesis Tag Resource API
  slug: kinesis-tag-resource-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kinesis/openapi/kinesis-tag-resource-api-openapi.yml
- filename: kinesis-untag-resource-api-openapi.yml
  format: yaml
  label: AWS Kinesis Untag Resource API
  slug: kinesis-untag-resource-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kinesis/openapi/kinesis-untag-resource-api-openapi.yml
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
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: AWS Kinesis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AWS Kinesis, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: AWS Kinesis
provider_slug: kinesis
slug: kinesis-domain-security
source_filename: kinesis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/kinesis/security/kinesis-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Analytics
- Apache Flink
- Amazon Web Services
- Big Data
- Data Processing
- Real-Time
- Streaming
- Video
---
