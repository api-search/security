---
api_specs:
- filename: decodable-openapi.yml
  format: yaml
  label: Decodable Connections API
  slug: decodable-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/decodable/refs/heads/main/openapi/decodable-openapi.yml
- filename: decodable-openapi.yml
  format: yaml
  label: Decodable Streams API
  slug: decodable-streams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/decodable/refs/heads/main/openapi/decodable-openapi.yml
- filename: decodable-openapi.yml
  format: yaml
  label: Decodable Pipelines API
  slug: decodable-pipelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/decodable/refs/heads/main/openapi/decodable-openapi.yml
- filename: decodable-openapi.yml
  format: yaml
  label: Decodable Secrets API
  slug: decodable-secrets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/decodable/refs/heads/main/openapi/decodable-openapi.yml
- filename: decodable-openapi.yml
  format: yaml
  label: Decodable Resources API
  slug: decodable-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/decodable/refs/heads/main/openapi/decodable-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: decodable.co
  spf: true
hosts:
- cert_expires: Sep  9 23:46:06 2026 GMT
  host: www.decodable.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 26 23:59:59 2027 GMT
  host: docs.decodable.co
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: <account>.api.decodable.co
  https: false
kind: domain-security
layout: security
method: probed
name: Decodable Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Decodable, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Decodable
provider_slug: decodable
slug: decodable-domain-security
source_filename: decodable-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.decodable.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 23:46:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.decodable.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 23:59:59 2027 GMT\n  hsts: false\n- host: <account>.api.decodable.co\n  https: false\ndomains:\n- domain: decodable.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/decodable/refs/heads/main/security/decodable-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Stream Processing
- Apache Flink
- Debezium
- Real Time Data
- Data Pipelines
- CDC
---
