---
api_specs:
- filename: aws-api-gateway-apikeys-api-openapi.yml
  format: yaml
  label: Amazon API Gateway ApiKeys API
  slug: aws-api-gateway-apikeys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/openapi/aws-api-gateway-apikeys-api-openapi.yml
- filename: aws-api-gateway-apis-api-openapi.yml
  format: yaml
  label: Amazon API Gateway Apis API
  slug: aws-api-gateway-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/openapi/aws-api-gateway-apis-api-openapi.yml
- filename: aws-api-gateway-authorizers-api-openapi.yml
  format: yaml
  label: Amazon API Gateway Authorizers API
  slug: aws-api-gateway-authorizers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/openapi/aws-api-gateway-authorizers-api-openapi.yml
- filename: aws-api-gateway-connections-api-openapi.yml
  format: yaml
  label: Amazon API Gateway Connections API
  slug: aws-api-gateway-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/openapi/aws-api-gateway-connections-api-openapi.yml
- filename: aws-api-gateway-deployments-api-openapi.yml
  format: yaml
  label: Amazon API Gateway Deployments API
  slug: aws-api-gateway-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/openapi/aws-api-gateway-deployments-api-openapi.yml
- filename: aws-api-gateway-integrations-api-openapi.yml
  format: yaml
  label: Amazon API Gateway Integrations API
  slug: aws-api-gateway-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/openapi/aws-api-gateway-integrations-api-openapi.yml
- filename: aws-api-gateway-methods-api-openapi.yml
  format: yaml
  label: Amazon API Gateway Methods API
  slug: aws-api-gateway-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/openapi/aws-api-gateway-methods-api-openapi.yml
- filename: aws-api-gateway-resources-api-openapi.yml
  format: yaml
  label: Amazon API Gateway Resources API
  slug: aws-api-gateway-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/openapi/aws-api-gateway-resources-api-openapi.yml
- filename: aws-api-gateway-restapis-api-openapi.yml
  format: yaml
  label: Amazon API Gateway RestApis API
  slug: aws-api-gateway-restapis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/openapi/aws-api-gateway-restapis-api-openapi.yml
- filename: aws-api-gateway-routes-api-openapi.yml
  format: yaml
  label: Amazon API Gateway Routes API
  slug: aws-api-gateway-routes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/openapi/aws-api-gateway-routes-api-openapi.yml
- filename: aws-api-gateway-stages-api-openapi.yml
  format: yaml
  label: Amazon API Gateway Stages API
  slug: aws-api-gateway-stages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/openapi/aws-api-gateway-stages-api-openapi.yml
- filename: aws-api-gateway-usageplans-api-openapi.yml
  format: yaml
  label: Amazon API Gateway UsagePlans API
  slug: aws-api-gateway-usageplans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/openapi/aws-api-gateway-usageplans-api-openapi.yml
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
name: Aws Api Gateway Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon API Gateway, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amazon API Gateway
provider_slug: aws-api-gateway
slug: aws-api-gateway-domain-security
source_filename: aws-api-gateway-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: docs.aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/security/aws-api-gateway-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- API Gateway
- Cloud
- REST
- HTTP
- WebSocket
- Serverless
- MCP
- AgentCore
- Developer Portal
---
