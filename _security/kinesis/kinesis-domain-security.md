---
api_specs:
- filename: amazon-kinesis-data-streams-openapi-original.yml
  format: yaml
  label: Amazon Kinesis Data Streams API
  slug: data-streams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kinesis/refs/heads/main/openapi/amazon-kinesis-data-streams-openapi-original.yml
- filename: amazon-data-firehose-openapi-original.yml
  format: yaml
  label: Amazon Data Firehose API
  slug: data-firehose-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kinesis/refs/heads/main/openapi/amazon-data-firehose-openapi-original.yml
- filename: amazon-kinesis-data-analytics-openapi-original.yml
  format: yaml
  label: Amazon Kinesis Data Analytics API
  slug: data-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kinesis/refs/heads/main/openapi/amazon-kinesis-data-analytics-openapi-original.yml
- filename: amazon-kinesis-video-streams-openapi-original.yml
  format: yaml
  label: Amazon Kinesis Video Streams API
  slug: video-streams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kinesis/refs/heads/main/openapi/amazon-kinesis-video-streams-openapi-original.yml
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
kind: domain-security
layout: security
method: probed
name: Kinesis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AWS Kinesis, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: AWS Kinesis
provider_slug: kinesis
slug: kinesis-domain-security
source_filename: kinesis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kinesis/refs/heads/main/security/kinesis-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Analytics
- Apache Flink
- Big Data
- Data Processing
- Real-Time
- Streaming
- Video
---
