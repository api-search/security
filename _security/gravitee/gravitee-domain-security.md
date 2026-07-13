---
api_specs:
- filename: gravitee-apim-openapi.yml
  format: yaml
  label: Gravitee API Management
  slug: gravitee-api-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gravitee/refs/heads/main/openapi/gravitee-apim-openapi.yml
- filename: gravitee-am-openapi.yml
  format: yaml
  label: Gravitee Access Management
  slug: gravitee-access-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gravitee/refs/heads/main/openapi/gravitee-am-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gravitee.io
  spf: true
hosts:
- cert_expires: Sep 24 16:09:18 2026 GMT
  host: www.gravitee.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 13:32:41 2026 GMT
  host: documentation.gravitee.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 19 04:09:17 2026 GMT
  host: cockpit.gravitee.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gravitee Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gravitee, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Gravitee
provider_slug: gravitee
slug: gravitee-domain-security
source_filename: gravitee-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gravitee.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 16:09:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: documentation.gravitee.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 13:32:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: cockpit.gravitee.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 04:09:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: gravitee.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gravitee/refs/heads/main/security/gravitee-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- API Gateway
- API Management
- Access Management
- Identity
- Event-Driven
- Event Management
- Kafka Gateway
- Kafka
- MQTT
- GraphQL
- gRPC
- AI Gateway
- MCP
- A2A
- LLM Proxy
- Multi-Gateway Federation
- Developer Portal
- Open Source
- Apache 2.0
---
