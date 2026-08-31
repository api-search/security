---
api_specs:
- filename: jodo-webhooks-asyncapi.yml
  format: yaml
  label: Jodo Webhooks
  slug: jodo-webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/jodo/refs/heads/main/asyncapi/jodo-webhooks-asyncapi.yml
- filename: jodo-configuration-api-openapi.yml
  format: yaml
  label: Jodo Configuration API
  slug: jodo-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jodo/refs/heads/main/openapi/jodo-configuration-api-openapi.yml
- filename: jodo-flex-api-openapi.yml
  format: yaml
  label: Jodo Flex API
  slug: jodo-flex-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jodo/refs/heads/main/openapi/jodo-flex-api-openapi.yml
- filename: jodo-pay-api-openapi.yml
  format: yaml
  label: Jodo Pay API
  slug: jodo-pay-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jodo/refs/heads/main/openapi/jodo-pay-api-openapi.yml
- filename: jodo-students-api-openapi.yml
  format: yaml
  label: Jodo Students API
  slug: jodo-students-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jodo/refs/heads/main/openapi/jodo-students-api-openapi.yml
- filename: jodo-users-api-openapi.yml
  format: yaml
  label: Jodo Users API
  slug: jodo-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jodo/refs/heads/main/openapi/jodo-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: jodo.in
  spf: false
hosts:
- cert_expires: Feb  8 23:59:59 2027 GMT
  host: www.jodo.in
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  8 23:59:59 2027 GMT
  host: docs.jodo.in
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 31 23:59:59 2027 GMT
  host: ext.jodo.in
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jodo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jodo, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Jodo
provider_slug: jodo
slug: jodo-domain-security
source_filename: jodo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.jodo.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  8 23:59:59 2027 GMT\n  hsts: false\n- host: docs.jodo.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  8 23:59:59 2027 GMT\n  hsts: false\n- host: ext.jodo.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: jodo.in\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jodo/refs/heads/main/security/jodo-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Payments
- Education
- Fintech
- Fee Collection
- Lending
- India
- Webhook
- ERP Integration
- Financial-Services
---
