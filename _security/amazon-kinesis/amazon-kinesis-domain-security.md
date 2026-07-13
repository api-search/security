---
api_specs:
- filename: amazon-kinesis-data-streams-openapi.yml
  format: yaml
  label: Amazon Kinesis Data Streams
  slug: amazon-kinesis-data-streams
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-kinesis/refs/heads/main/openapi/amazon-kinesis-data-streams-openapi.yml
- filename: openapi.yaml
  format: yaml
  label: Amazon Data Firehose
  slug: amazon-data-firehose
  spec_type: OpenAPI
  url: https://api.apis.guru/v2/specs/amazonaws.com/firehose/2015-08-04/openapi.yaml
- filename: openapi.yaml
  format: yaml
  label: Amazon Managed Service for Apache Flink
  slug: amazon-managed-service-for-apache-flink
  spec_type: OpenAPI
  url: https://api.apis.guru/v2/specs/amazonaws.com/kinesisanalyticsv2/2018-05-23/openapi.yaml
- filename: openapi.yaml
  format: yaml
  label: Amazon Kinesis Video Streams
  slug: amazon-kinesis-video-streams
  spec_type: OpenAPI
  url: https://api.apis.guru/v2/specs/amazonaws.com/kinesisvideo/2017-09-30/openapi.yaml
- filename: openapi.yaml
  format: yaml
  label: Amazon Kinesis Video Streams Media
  slug: amazon-kinesis-video-streams-media
  spec_type: OpenAPI
  url: https://api.apis.guru/v2/specs/amazonaws.com/kinesis-video-media/2017-09-30/openapi.yaml
- filename: openapi.yaml
  format: yaml
  label: Amazon Kinesis Video Streams Archived Media
  slug: amazon-kinesis-video-streams-archived-media
  spec_type: OpenAPI
  url: https://api.apis.guru/v2/specs/amazonaws.com/kinesis-video-archived-media/2017-09-30/openapi.yaml
- filename: openapi.yaml
  format: yaml
  label: Amazon Kinesis Video Signaling Channels
  slug: amazon-kinesis-video-signaling-channels
  spec_type: OpenAPI
  url: https://api.apis.guru/v2/specs/amazonaws.com/kinesis-video-signaling/2019-12-04/openapi.yaml
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
