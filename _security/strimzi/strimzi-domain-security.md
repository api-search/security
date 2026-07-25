---
api_specs:
- filename: strimzi-consumer-api-openapi.yml
  format: yaml
  label: Strimzi Consumer API
  slug: strimzi-consumer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/strimzi/refs/heads/main/openapi/strimzi-consumer-api-openapi.yml
- filename: strimzi-producer-api-openapi.yml
  format: yaml
  label: Strimzi Producer API
  slug: strimzi-producer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/strimzi/refs/heads/main/openapi/strimzi-producer-api-openapi.yml
- filename: strimzi-seek-api-openapi.yml
  format: yaml
  label: Strimzi Seek API
  slug: strimzi-seek-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/strimzi/refs/heads/main/openapi/strimzi-seek-api-openapi.yml
- filename: strimzi-topics-api-openapi.yml
  format: yaml
  label: Strimzi Topics API
  slug: strimzi-topics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/strimzi/refs/heads/main/openapi/strimzi-topics-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: strimzi.io
  spf: false
hosts:
- cert_expires: Sep 12 16:28:26 2026 GMT
  host: strimzi.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Strimzi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Strimzi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Strimzi
provider_slug: strimzi
slug: strimzi-domain-security
source_filename: strimzi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: strimzi.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 16:28:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: strimzi.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/strimzi/refs/heads/main/security/strimzi-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Kafka
- Kubernetes
- Messaging
- Operator
- Streaming
---
