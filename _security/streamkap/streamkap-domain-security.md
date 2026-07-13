---
api_specs:
- filename: streamkap-openapi.yml
  format: yaml
  label: Streamkap Sources API
  slug: streamkap-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/streamkap/refs/heads/main/openapi/streamkap-openapi.yml
- filename: streamkap-openapi.yml
  format: yaml
  label: Streamkap Destinations API
  slug: streamkap-destinations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/streamkap/refs/heads/main/openapi/streamkap-openapi.yml
- filename: streamkap-openapi.yml
  format: yaml
  label: Streamkap Pipelines API
  slug: streamkap-pipelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/streamkap/refs/heads/main/openapi/streamkap-openapi.yml
- filename: streamkap-openapi.yml
  format: yaml
  label: Streamkap Connectors API
  slug: streamkap-connectors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/streamkap/refs/heads/main/openapi/streamkap-openapi.yml
- filename: streamkap-openapi.yml
  format: yaml
  label: Streamkap Transforms API
  slug: streamkap-transforms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/streamkap/refs/heads/main/openapi/streamkap-openapi.yml
- filename: streamkap-openapi.yml
  format: yaml
  label: Streamkap Topics API
  slug: streamkap-topics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/streamkap/refs/heads/main/openapi/streamkap-openapi.yml
- filename: streamkap-openapi.yml
  format: yaml
  label: Streamkap Tags API
  slug: streamkap-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/streamkap/refs/heads/main/openapi/streamkap-openapi.yml
- filename: streamkap-openapi.yml
  format: yaml
  label: Streamkap Kafka Access API
  slug: streamkap-kafka-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/streamkap/refs/heads/main/openapi/streamkap-openapi.yml
- filename: streamkap-openapi.yml
  format: yaml
  label: Streamkap Authentication API
  slug: streamkap-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/streamkap/refs/heads/main/openapi/streamkap-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: streamkap.com
  spf: true
hosts:
- cert_expires: Aug 22 18:01:46 2026 GMT
  host: streamkap.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 11 11:05:23 2026 GMT
  host: docs.streamkap.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 20 23:59:59 2027 GMT
  host: api.streamkap.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Streamkap Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Streamkap, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Streamkap
provider_slug: streamkap
slug: streamkap-domain-security
source_filename: streamkap-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: streamkap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 18:01:46 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.streamkap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 11 11:05:23 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.streamkap.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 20 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: streamkap.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/streamkap/refs/heads/main/security/streamkap-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Streaming
- ETL
- CDC
- Kafka
- Flink
- Data Integration
- Real Time
---
