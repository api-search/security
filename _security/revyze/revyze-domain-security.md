---
api_specs:
- filename: revyze-admin-api-openapi.yml
  format: yaml
  label: Revyze Admin API
  slug: revyze-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revyze/refs/heads/main/openapi/revyze-admin-api-openapi.yml
- filename: revyze-coach-api-openapi.yml
  format: yaml
  label: Revyze Coach API
  slug: revyze-coach-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revyze/refs/heads/main/openapi/revyze-coach-api-openapi.yml
- filename: revyze-fastapi-api-openapi.yml
  format: yaml
  label: Revyze FastAPI API
  slug: revyze-fastapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revyze/refs/heads/main/openapi/revyze-fastapi-api-openapi.yml
- filename: revyze-force-upgrade-app-api-openapi.yml
  format: yaml
  label: Revyze Force Upgrade App API
  slug: revyze-force-upgrade-app-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revyze/refs/heads/main/openapi/revyze-force-upgrade-app-api-openapi.yml
- filename: revyze-graphql3-api-openapi.yml
  format: yaml
  label: Revyze Graphql3 API
  slug: revyze-graphql3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revyze/refs/heads/main/openapi/revyze-graphql3-api-openapi.yml
- filename: revyze-health-api-openapi.yml
  format: yaml
  label: Revyze Health API
  slug: revyze-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revyze/refs/heads/main/openapi/revyze-health-api-openapi.yml
- filename: revyze-multiplayer-api-openapi.yml
  format: yaml
  label: Revyze Multiplayer API
  slug: revyze-multiplayer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revyze/refs/heads/main/openapi/revyze-multiplayer-api-openapi.yml
- filename: revyze-privacy-policy-api-openapi.yml
  format: yaml
  label: Revyze Privacy Policy API
  slug: revyze-privacy-policy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revyze/refs/heads/main/openapi/revyze-privacy-policy-api-openapi.yml
- filename: revyze-privacy-policy-en-api-openapi.yml
  format: yaml
  label: Revyze Privacy Policy En API
  slug: revyze-privacy-policy-en-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revyze/refs/heads/main/openapi/revyze-privacy-policy-en-api-openapi.yml
- filename: revyze-webhook-api-openapi.yml
  format: yaml
  label: Revyze Webhook API
  slug: revyze-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revyze/refs/heads/main/openapi/revyze-webhook-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: revyze.fr
  spf: true
hosts:
- cert_expires: Oct  5 15:08:39 2026 GMT
  host: www.revyze.fr
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 23:59:59 2026 GMT
  host: api.revyze.fr
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Revyze Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Revyze, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Revyze
provider_slug: revyze
slug: revyze-domain-security
source_filename: revyze-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.revyze.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 15:08:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.revyze.fr\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 10 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: revyze.fr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/revyze/refs/heads/main/security/revyze-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- EdTech
- Education
- Mobile
- Video
- Learning
- Quiz
- France
- GraphQL
---
