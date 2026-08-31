---
api_specs:
- filename: validic-devices-api-openapi.yml
  format: yaml
  label: Validic Devices API
  slug: validic-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/validic/refs/heads/main/openapi/validic-devices-api-openapi.yml
- filename: validic-marketplace-connections-api-openapi.yml
  format: yaml
  label: Validic Marketplace & Connections API
  slug: validic-marketplace-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/validic/refs/heads/main/openapi/validic-marketplace-connections-api-openapi.yml
- filename: validic-observations-data-api-openapi.yml
  format: yaml
  label: Validic Observations & Data API
  slug: validic-observations-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/validic/refs/heads/main/openapi/validic-observations-data-api-openapi.yml
- filename: validic-push-service-api-openapi.yml
  format: yaml
  label: Validic Push Service API
  slug: validic-push-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/validic/refs/heads/main/openapi/validic-push-service-api-openapi.yml
- filename: validic-streaming-api-openapi.yml
  format: yaml
  label: Validic Streaming API
  slug: validic-streaming-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/validic/refs/heads/main/openapi/validic-streaming-api-openapi.yml
- filename: validic-users-api-openapi.yml
  format: yaml
  label: Validic Users API
  slug: validic-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/validic/refs/heads/main/openapi/validic-users-api-openapi.yml
- filename: validic-measurements-api-openapi.yml
  format: yaml
  label: Validic Measurements API
  slug: validic-measurements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/validic/refs/heads/main/openapi/validic-measurements-api-openapi.yml
- filename: validic-organizations-api-openapi.yml
  format: yaml
  label: Validic Organizations API
  slug: validic-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/validic/refs/heads/main/openapi/validic-organizations-api-openapi.yml
- filename: validic-streams-api-openapi.yml
  format: yaml
  label: Validic Streams API
  slug: validic-streams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/validic/refs/heads/main/openapi/validic-streams-api-openapi.yml
- filename: validic-streams-token-token-api-openapi.yml
  format: yaml
  label: Validic Streams?token={token} API
  slug: validic-streams-token-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/validic/refs/heads/main/openapi/validic-streams-token-token-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: validic.com
  spf: true
hosts:
- cert_expires: Sep 30 23:59:59 2026 GMT
  host: validic.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 22:54:33 2026 GMT
  host: developer.validic.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  7 23:59:59 2026 GMT
  host: api.v2.validic.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Validic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Validic, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Validic
provider_slug: validic
slug: validic-domain-security
source_filename: validic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: validic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.validic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 22:54:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.v2.validic.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  7 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: validic.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/validic/refs/heads/main/security/validic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Health Data
- Digital Health
- Wearables
- Remote Patient Monitoring
- Health IoT
- Interoperability
- HIPAA
---
