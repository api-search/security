---
api_specs:
- filename: streamnative-cloudstreamnativeio-v1alpha1-api-openapi.yml
  format: yaml
  label: StreamNative Cloud Streamnative Io V1alpha1 API
  slug: streamnative-cloudstreamnativeio-v1alpha1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/streamnative/refs/heads/main/openapi/streamnative-cloudstreamnativeio-v1alpha1-api-openapi.yml
- filename: streamnative-ksn-consumer-group-api-openapi.yml
  format: yaml
  label: StreamNative Ksn Consumer Group API
  slug: streamnative-ksn-consumer-group-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/streamnative/refs/heads/main/openapi/streamnative-ksn-consumer-group-api-openapi.yml
- filename: streamnative-ksn-topics-api-openapi.yml
  format: yaml
  label: StreamNative Ksn Topics API
  slug: streamnative-ksn-topics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/streamnative/refs/heads/main/openapi/streamnative-ksn-topics-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: streamnative.io
  spf: true
- caa:
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: streamnative.cloud
  spf: true
hosts:
- cert_expires: Dec 31 07:37:19 2026 GMT
  host: streamnative.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  4 12:10:52 2026 GMT
  host: docs.streamnative.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 22:33:52 2026 GMT
  host: api.streamnative.cloud
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Streamnative Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for StreamNative, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: StreamNative
provider_slug: streamnative
slug: streamnative-domain-security
source_filename: streamnative-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: streamnative.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 07:37:19 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.streamnative.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 12:10:52 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.streamnative.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 22:33:52 2026 GMT\n  hsts: null\ndomains:\n- domain: streamnative.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: streamnative.cloud\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/streamnative/refs/heads/main/security/streamnative-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Data Streaming
- Apache Pulsar
- Apache Kafka
- Messaging
- Event Streaming
- Cloud
---
