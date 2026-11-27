---
api_specs:
- filename: apigee-hybrid-api-openapi.yml
  format: yaml
  label: Apigee Hybrid API
  slug: apigee-hybrid-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apigee/openapi/apigee-hybrid-api-openapi.yml
- filename: apigee-organizations-api-openapi.yml
  format: yaml
  label: Apigee Organizations API
  slug: apigee-organizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apigee/openapi/apigee-organizations-api-openapi.yml
- filename: apigee-projects-api-openapi.yml
  format: yaml
  label: Apigee Projects API
  slug: apigee-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apigee/openapi/apigee-projects-api-openapi.yml
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
- cert_expires: Dec  3 19:21:52 2026 GMT
  host: cloud.google.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  3 19:23:22 2026 GMT
  host: apigee.googleapis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  3 19:23:22 2026 GMT
  host: apigeeconnect.googleapis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
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
source_yaml: "generated: '2026-10-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cloud.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 19:21:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: apigee.googleapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 19:23:22 2026 GMT\n  hsts: null\n- host: apigeeconnect.googleapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 19:23:22 2026 GMT\n  hsts: null\ndomains:\n- domain: google.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: googleapis.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/apigee/security/apigee-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Apigee
- Advanced API Security
- AI Agents
- Analytics
- API Gateway
- API Governance
- API Hub
- API Management
- Developer Portal
- Enterprise
- Generative AI
- Hybrid
- Integration
- Microservices
- MCP
- Monetization
---
