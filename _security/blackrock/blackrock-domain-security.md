---
api_specs:
- filename: blackrock-authorizationurl-generate-api-openapi.yml
  format: yaml
  label: BlackRock Authorization Url:generate API
  slug: blackrock-authorizationurl-generate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blackrock/refs/heads/main/openapi/blackrock-authorizationurl-generate-api-openapi.yml
- filename: blackrock-studionotifications-api-openapi.yml
  format: yaml
  label: BlackRock Studio Notifications API
  slug: blackrock-studionotifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blackrock/refs/heads/main/openapi/blackrock-studionotifications-api-openapi.yml
- filename: blackrock-studionotifications-batchcreate-api-openapi.yml
  format: yaml
  label: BlackRock Studio Notifications:batch Create API
  slug: blackrock-studionotifications-batchcreate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blackrock/refs/heads/main/openapi/blackrock-studionotifications-batchcreate-api-openapi.yml
- filename: blackrock-studionotifications-filter-api-openapi.yml
  format: yaml
  label: BlackRock Studio Notifications:filter API
  slug: blackrock-studionotifications-filter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blackrock/refs/heads/main/openapi/blackrock-studionotifications-filter-api-openapi.yml
- filename: blackrock-studiosubscriptions-api-openapi.yml
  format: yaml
  label: BlackRock Studio Subscriptions API
  slug: blackrock-studiosubscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blackrock/refs/heads/main/openapi/blackrock-studiosubscriptions-api-openapi.yml
- filename: blackrock-studiosubscriptions-batchcreate-api-openapi.yml
  format: yaml
  label: BlackRock Studio Subscriptions:batch Create API
  slug: blackrock-studiosubscriptions-batchcreate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blackrock/refs/heads/main/openapi/blackrock-studiosubscriptions-batchcreate-api-openapi.yml
- filename: blackrock-studiosubscriptions-filter-api-openapi.yml
  format: yaml
  label: BlackRock Studio Subscriptions:filter API
  slug: blackrock-studiosubscriptions-filter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blackrock/refs/heads/main/openapi/blackrock-studiosubscriptions-filter-api-openapi.yml
- filename: blackrock-token-checktokenexists-api-openapi.yml
  format: yaml
  label: BlackRock Token:check Token Exists API
  slug: blackrock-token-checktokenexists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blackrock/refs/heads/main/openapi/blackrock-token-checktokenexists-api-openapi.yml
- filename: blackrock-token-generate-api-openapi.yml
  format: yaml
  label: BlackRock Token:generate API
  slug: blackrock-token-generate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blackrock/refs/heads/main/openapi/blackrock-token-generate-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: blackrock.com
  spf: true
hosts:
- cert_expires: Mar  4 23:59:59 2027 GMT
  host: www.blackrock.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Blackrock Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BlackRock, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: BlackRock
provider_slug: blackrock
slug: blackrock-domain-security
source_filename: blackrock-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.blackrock.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  4 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: blackrock.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blackrock/refs/heads/main/security/blackrock-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Asset Management
- Finance
- Fintech
- Investment Management
- Portfolio Management
- Risk Analytics
- Fortune 500
---
