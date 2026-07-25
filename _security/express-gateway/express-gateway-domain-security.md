---
api_specs:
- filename: express-gateway-apps-api-openapi.yml
  format: yaml
  label: Express Gateway Apps API
  slug: express-gateway-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/express-gateway/refs/heads/main/openapi/express-gateway-apps-api-openapi.yml
- filename: express-gateway-credentials-api-openapi.yml
  format: yaml
  label: Express Gateway Credentials API
  slug: express-gateway-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/express-gateway/refs/heads/main/openapi/express-gateway-credentials-api-openapi.yml
- filename: express-gateway-scopes-api-openapi.yml
  format: yaml
  label: Express Gateway Scopes API
  slug: express-gateway-scopes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/express-gateway/refs/heads/main/openapi/express-gateway-scopes-api-openapi.yml
- filename: express-gateway-users-api-openapi.yml
  format: yaml
  label: Express Gateway Users API
  slug: express-gateway-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/express-gateway/refs/heads/main/openapi/express-gateway-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: express-gateway.io
  spf: false
hosts:
- cert_expires: Sep  4 08:46:33 2026 GMT
  host: www.express-gateway.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Express Gateway Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Express Gateway, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Express Gateway
provider_slug: express-gateway
slug: express-gateway-domain-security
source_filename: express-gateway-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.express-gateway.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 08:46:33 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: express-gateway.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/express-gateway/refs/heads/main/security/express-gateway-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- API Composition
- API Gateway
- BFF
---
