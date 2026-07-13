---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Amazon Kinesis Video Streams API
  slug: amazon-kinesis-video-streams-api
  spec_type: OpenAPI
  url: https://api.apis.guru/v2/specs/amazonaws.com/kinesisvideo/2017-09-30/openapi.yaml
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
- host: kinesisvideo.amazonaws.com
  https: false
- cert_expires: Dec 19 23:59:59 2026 GMT
  host: kinesisvideo.us-east-1.amazonaws.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Amazon Kinesis Video Streams Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon Kinesis Video Streams, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amazon Kinesis Video Streams
provider_slug: amazon-kinesis-video-streams
slug: amazon-kinesis-video-streams-domain-security
source_filename: amazon-kinesis-video-streams-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: kinesisvideo.amazonaws.com\n  https: false\n- host: kinesisvideo.us-east-1.amazonaws.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: amazonaws.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-kinesis-video-streams/refs/heads/main/security/amazon-kinesis-video-streams-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- IoT
- Machine Learning
- Media
- Video Streaming
---
