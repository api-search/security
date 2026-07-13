---
api_specs:
- filename: apigee-api-management-openapi.yml
  format: yaml
  label: Apigee API Management
  slug: apigee-api-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apigee/refs/heads/main/openapi/apigee-api-management-openapi.yml
- filename: apigee-api-hub-openapi.yml
  format: yaml
  label: Apigee API Hub API
  slug: apigee-api-hub-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apigee/refs/heads/main/openapi/apigee-api-hub-openapi.yml
- filename: apigee-integrations-openapi.yml
  format: yaml
  label: Apigee Integrations API
  slug: apigee-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apigee/refs/heads/main/openapi/apigee-integrations-openapi.yml
- filename: apigee-apim-openapi.yml
  format: yaml
  label: Apigee API Management API
  slug: apigee-api-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apigee/refs/heads/main/openapi/apigee-apim-openapi.yml
- filename: apigee-registry-openapi.yml
  format: yaml
  label: Apigee Registry API
  slug: apigee-registry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apigee/refs/heads/main/openapi/apigee-registry-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: google.com
  spf: true
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: googleapis.com
  spf: true
hosts:
- cert_expires: Sep 14 08:35:22 2026 GMT
  host: cloud.google.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 08:37:17 2026 GMT
  host: apigee.googleapis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 08:37:17 2026 GMT
  host: apihub.googleapis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Apigee Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apigee, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Apigee
provider_slug: apigee
slug: apigee-domain-security
source_filename: apigee-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cloud.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:35:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: apigee.googleapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:37:17 2026 GMT\n  hsts: null\n- host: apihub.googleapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:37:17 2026 GMT\n  hsts: null\ndomains:\n- domain: google.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: googleapis.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apigee/refs/heads/main/security/apigee-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Advanced API Security
- Agentic AI
- Analytics
- API Gateway
- API Governance
- API Hub
- API Management
- Developer Portal
- Enterprise
- Generative AI
- Hybrid
- Integrations
- Microservices
- MCP
- Model Context Protocol
- Monetization
---
