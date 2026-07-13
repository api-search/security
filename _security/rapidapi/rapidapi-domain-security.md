---
api_specs:
- filename: rapidapi-rest-platform-api-openapi.yml
  format: yaml
  label: RapidAPI REST Platform API
  slug: rapidapi-rest-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rapidapi/refs/heads/main/openapi/rapidapi-rest-platform-api-openapi.yml
- filename: rapidapi-graphql-platform-api-openapi.yml
  format: yaml
  label: RapidAPI GraphQL Platform API
  slug: rapidapi-graphql-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rapidapi/refs/heads/main/openapi/rapidapi-graphql-platform-api-openapi.yml
- filename: rapidapi-hub-api-openapi.yml
  format: yaml
  label: RapidAPI Hub API
  slug: rapidapi-hub-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rapidapi/refs/heads/main/openapi/rapidapi-hub-api-openapi.yml
- filename: rapidapi-testing-api-openapi.yml
  format: yaml
  label: RapidAPI Testing API
  slug: rapidapi-testing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rapidapi/refs/heads/main/openapi/rapidapi-testing-api-openapi.yml
- filename: rapidapi-studio-api-openapi.yml
  format: yaml
  label: RapidAPI Studio API
  slug: rapidapi-studio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rapidapi/refs/heads/main/openapi/rapidapi-studio-api-openapi.yml
- filename: rapidapi-gateway-api-openapi.yml
  format: yaml
  label: RapidAPI Gateway API
  slug: rapidapi-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rapidapi/refs/heads/main/openapi/rapidapi-gateway-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: rapidapi.com
  spf: true
hosts:
- cert_expires: Sep 18 08:42:50 2026 GMT
  host: rapidapi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 08:49:03 2026 GMT
  host: docs.rapidapi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: gateway.rapidapi.com
  https: false
kind: domain-security
layout: security
method: probed
name: Rapidapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RapidAPI, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: RapidAPI
provider_slug: rapidapi
slug: rapidapi-domain-security
source_filename: rapidapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rapidapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 08:42:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.rapidapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 08:49:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: gateway.rapidapi.com\n  https: false\ndomains:\n- domain: rapidapi.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rapidapi/refs/heads/main/security/rapidapi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- API Marketplace
- API Management
- API Testing
- API Gateway
- API Design
- Enterprise
---
