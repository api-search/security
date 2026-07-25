---
api_specs:
- filename: amazon-api-gateway-websocket-asyncapi.yml
  format: yaml
  label: Amazon API Gateway WebSocket API
  slug: websocket-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-api-gateway/refs/heads/main/asyncapi/amazon-api-gateway-websocket-asyncapi.yml
- filename: amazon-api-gateway-api-keys-api-openapi.yml
  format: yaml
  label: Amazon API Gateway API Keys API
  slug: amazon-api-gateway-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-api-gateway/refs/heads/main/openapi/amazon-api-gateway-api-keys-api-openapi.yml
- filename: amazon-api-gateway-authorizers-api-openapi.yml
  format: yaml
  label: Amazon API Gateway Authorizers API
  slug: amazon-api-gateway-authorizers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-api-gateway/refs/heads/main/openapi/amazon-api-gateway-authorizers-api-openapi.yml
- filename: amazon-api-gateway-base-path-mappings-api-openapi.yml
  format: yaml
  label: Amazon API Gateway Base Path Mappings API
  slug: amazon-api-gateway-base-path-mappings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-api-gateway/refs/heads/main/openapi/amazon-api-gateway-base-path-mappings-api-openapi.yml
- filename: amazon-api-gateway-deployments-api-openapi.yml
  format: yaml
  label: Amazon API Gateway Deployments API
  slug: amazon-api-gateway-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-api-gateway/refs/heads/main/openapi/amazon-api-gateway-deployments-api-openapi.yml
- filename: amazon-api-gateway-documentation-api-openapi.yml
  format: yaml
  label: Amazon API Gateway Documentation API
  slug: amazon-api-gateway-documentation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-api-gateway/refs/heads/main/openapi/amazon-api-gateway-documentation-api-openapi.yml
- filename: amazon-api-gateway-domain-names-api-openapi.yml
  format: yaml
  label: Amazon API Gateway Domain Names API
  slug: amazon-api-gateway-domain-names-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-api-gateway/refs/heads/main/openapi/amazon-api-gateway-domain-names-api-openapi.yml
- filename: amazon-api-gateway-gateway-responses-api-openapi.yml
  format: yaml
  label: Amazon API Gateway Gateway Responses API
  slug: amazon-api-gateway-gateway-responses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-api-gateway/refs/heads/main/openapi/amazon-api-gateway-gateway-responses-api-openapi.yml
- filename: amazon-api-gateway-methods-api-openapi.yml
  format: yaml
  label: Amazon API Gateway Methods API
  slug: amazon-api-gateway-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-api-gateway/refs/heads/main/openapi/amazon-api-gateway-methods-api-openapi.yml
- filename: amazon-api-gateway-models-api-openapi.yml
  format: yaml
  label: Amazon API Gateway Models API
  slug: amazon-api-gateway-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-api-gateway/refs/heads/main/openapi/amazon-api-gateway-models-api-openapi.yml
- filename: amazon-api-gateway-request-validators-api-openapi.yml
  format: yaml
  label: Amazon API Gateway Request Validators API
  slug: amazon-api-gateway-request-validators-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-api-gateway/refs/heads/main/openapi/amazon-api-gateway-request-validators-api-openapi.yml
- filename: amazon-api-gateway-resources-api-openapi.yml
  format: yaml
  label: Amazon API Gateway Resources API
  slug: amazon-api-gateway-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-api-gateway/refs/heads/main/openapi/amazon-api-gateway-resources-api-openapi.yml
- filename: amazon-api-gateway-rest-apis-api-openapi.yml
  format: yaml
  label: Amazon API Gateway REST APIs API
  slug: amazon-api-gateway-rest-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-api-gateway/refs/heads/main/openapi/amazon-api-gateway-rest-apis-api-openapi.yml
- filename: amazon-api-gateway-stages-api-openapi.yml
  format: yaml
  label: Amazon API Gateway Stages API
  slug: amazon-api-gateway-stages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-api-gateway/refs/heads/main/openapi/amazon-api-gateway-stages-api-openapi.yml
- filename: amazon-api-gateway-usage-plans-api-openapi.yml
  format: yaml
  label: Amazon API Gateway Usage Plans API
  slug: amazon-api-gateway-usage-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-api-gateway/refs/heads/main/openapi/amazon-api-gateway-usage-plans-api-openapi.yml
- filename: amazon-api-gateway-vpc-links-api-openapi.yml
  format: yaml
  label: Amazon API Gateway VPC Links API
  slug: amazon-api-gateway-vpc-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-api-gateway/refs/heads/main/openapi/amazon-api-gateway-vpc-links-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amazon.com
  spf: true
hosts:
- cert_expires: Oct 17 23:59:59 2026 GMT
  host: aws.amazon.com
  hsts: true
  hsts_max_age: 47304000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  8 23:59:59 2026 GMT
  host: docs.aws.amazon.com
  hsts: true
  hsts_max_age: 47304000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Amazon Api Gateway Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon API Gateway, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amazon API Gateway
provider_slug: amazon-api-gateway
slug: amazon-api-gateway-domain-security
source_filename: amazon-api-gateway-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: docs.aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-api-gateway/refs/heads/main/security/amazon-api-gateway-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Gateway
- HTTP API
- REST API
- Serverless
- WebSocket
---
