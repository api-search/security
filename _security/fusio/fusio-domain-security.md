---
api_specs:
- filename: fusio-backend.json
  format: json
  label: Fusio Backend API
  slug: fusio-backend-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fusio/refs/heads/main/openapi/fusio-backend.json
- filename: fusio-consumer.json
  format: json
  label: Fusio Consumer API
  slug: fusio-consumer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fusio/refs/heads/main/openapi/fusio-consumer.json
- filename: fusio-system.json
  format: json
  label: Fusio System API
  slug: fusio-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fusio/refs/heads/main/openapi/fusio-system.json
- filename: fusio-authorization.json
  format: json
  label: Fusio Authorization API
  slug: fusio-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fusio/refs/heads/main/openapi/fusio-authorization.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: fusio-project.org
  spf: true
hosts:
- cert_expires: Nov  7 04:47:51 2026 GMT
  host: docs.fusio-project.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  4 11:14:03 2026 GMT
  host: www.fusio-project.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  6 13:34:38 2026 GMT
  host: demo.fusio-project.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fusio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fusio, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Fusio
provider_slug: fusio
slug: fusio-domain-security
source_filename: fusio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.fusio-project.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 04:47:51 2026 GMT\n  hsts: false\n- host: www.fusio-project.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 11:14:03 2026 GMT\n  hsts: false\n- host: demo.fusio-project.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 13:34:38 2026 GMT\n  hsts: false\ndomains:\n- domain: fusio-project.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fusio/refs/heads/main/security/fusio-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- API Management
- Open-Source
- REST API
- API Gateway
- Developer Portal
- OpenAPI
- Self-Hosted
- MCP
---
