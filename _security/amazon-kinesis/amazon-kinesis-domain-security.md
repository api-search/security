---
api_specs:
- filename: amazon-kinesis-account-api-openapi.yml
  format: yaml
  label: Amazon Kinesis Account API
  slug: amazon-kinesis-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-kinesis/refs/heads/main/openapi/amazon-kinesis-account-api-openapi.yml
- filename: amazon-kinesis-consumers-api-openapi.yml
  format: yaml
  label: Amazon Kinesis Consumers API
  slug: amazon-kinesis-consumers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-kinesis/refs/heads/main/openapi/amazon-kinesis-consumers-api-openapi.yml
- filename: amazon-kinesis-encryption-api-openapi.yml
  format: yaml
  label: Amazon Kinesis Encryption API
  slug: amazon-kinesis-encryption-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-kinesis/refs/heads/main/openapi/amazon-kinesis-encryption-api-openapi.yml
- filename: amazon-kinesis-monitoring-api-openapi.yml
  format: yaml
  label: Amazon Kinesis Monitoring API
  slug: amazon-kinesis-monitoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-kinesis/refs/heads/main/openapi/amazon-kinesis-monitoring-api-openapi.yml
- filename: amazon-kinesis-policies-api-openapi.yml
  format: yaml
  label: Amazon Kinesis Policies API
  slug: amazon-kinesis-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-kinesis/refs/heads/main/openapi/amazon-kinesis-policies-api-openapi.yml
- filename: amazon-kinesis-records-api-openapi.yml
  format: yaml
  label: Amazon Kinesis Records API
  slug: amazon-kinesis-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-kinesis/refs/heads/main/openapi/amazon-kinesis-records-api-openapi.yml
- filename: amazon-kinesis-shards-api-openapi.yml
  format: yaml
  label: Amazon Kinesis Shards API
  slug: amazon-kinesis-shards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-kinesis/refs/heads/main/openapi/amazon-kinesis-shards-api-openapi.yml
- filename: amazon-kinesis-streams-api-openapi.yml
  format: yaml
  label: Amazon Kinesis Streams API
  slug: amazon-kinesis-streams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-kinesis/refs/heads/main/openapi/amazon-kinesis-streams-api-openapi.yml
- filename: amazon-kinesis-x-amz-target-kinesis-20131202-addtagstostream-api-openapi.yml
  format: yaml
  label: 'Amazon Kinesis #X Amz Target=Kinesis 20131202.AddTagsToStream API'
  slug: amazon-kinesis-x-amz-target-kinesis-20131202-addtagstostream-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-kinesis/refs/heads/main/openapi/amazon-kinesis-x-amz-target-kinesis-20131202-addtagstostream-api-openapi.yml
- filename: amazon-kinesis-x-amz-target-kinesis-20131202-listtagsforstream-api-openapi.yml
  format: yaml
  label: 'Amazon Kinesis #X Amz Target=Kinesis 20131202.ListTagsForStream API'
  slug: amazon-kinesis-x-amz-target-kinesis-20131202-listtagsforstream-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-kinesis/refs/heads/main/openapi/amazon-kinesis-x-amz-target-kinesis-20131202-listtagsforstream-api-openapi.yml
- filename: amazon-kinesis-x-amz-target-kinesis-20131202-removetagsfromstream-api-openapi.yml
  format: yaml
  label: 'Amazon Kinesis #X Amz Target=Kinesis 20131202.RemoveTagsFromStream API'
  slug: amazon-kinesis-x-amz-target-kinesis-20131202-removetagsfromstream-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-kinesis/refs/heads/main/openapi/amazon-kinesis-x-amz-target-kinesis-20131202-removetagsfromstream-api-openapi.yml
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
- cert_expires: Oct 17 23:59:59 2026 GMT
  host: aws.amazon.com
  hsts: true
  hsts_max_age: 47304000
  https: true
  tls_version: TLSv1.3
- host: kinesis.amazonaws.com
  https: false
- host: firehose.amazonaws.com
  https: false
kind: domain-security
layout: security
method: probed
name: Amazon Kinesis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon Kinesis, probed live across 3 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amazon Kinesis
provider_slug: amazon-kinesis
slug: amazon-kinesis-domain-security
source_filename: amazon-kinesis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: kinesis.amazonaws.com\n  https: false\n- host: firehose.amazonaws.com\n  https: false\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: amazonaws.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-kinesis/refs/heads/main/security/amazon-kinesis-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Analytics
- Big Data
- Data Processing
- Real-Time
- Streaming
---
