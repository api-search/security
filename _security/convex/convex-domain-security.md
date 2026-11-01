---
api_specs:
- filename: convex-asyncapi.yml
  format: yaml
  label: Convex Sync Protocol
  slug: sync-protocol
  spec_type: AsyncAPI
  url: https://artifacts.apis.io/convex/asyncapi/convex-asyncapi.yml
- filename: convex-actions-api-openapi.yml
  format: yaml
  label: Convex Actions API
  slug: convex-actions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/convex/openapi/convex-actions-api-openapi.yml
- filename: convex-deployments-api-openapi.yml
  format: yaml
  label: Convex Deployments API
  slug: convex-deployments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/convex/openapi/convex-deployments-api-openapi.yml
- filename: convex-functions-api-openapi.yml
  format: yaml
  label: Convex Functions API
  slug: convex-functions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/convex/openapi/convex-functions-api-openapi.yml
- filename: convex-mutations-api-openapi.yml
  format: yaml
  label: Convex Mutations API
  slug: convex-mutations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/convex/openapi/convex-mutations-api-openapi.yml
- filename: convex-projects-api-openapi.yml
  format: yaml
  label: Convex Projects API
  slug: convex-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/convex/openapi/convex-projects-api-openapi.yml
- filename: convex-queries-api-openapi.yml
  format: yaml
  label: Convex Queries API
  slug: convex-queries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/convex/openapi/convex-queries-api-openapi.yml
- filename: convex-teams-api-openapi.yml
  format: yaml
  label: Convex Teams API
  slug: convex-teams-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/convex/openapi/convex-teams-api-openapi.yml
- filename: convex-access-tokens-api-openapi.yml
  format: yaml
  label: Convex Access Tokens API
  slug: convex-access-tokens-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/convex/openapi/convex-access-tokens-api-openapi.yml
- filename: convex-custom-domains-api-openapi.yml
  format: yaml
  label: Convex Custom Domains API
  slug: convex-custom-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/convex/openapi/convex-custom-domains-api-openapi.yml
- filename: convex-environment-variables-api-openapi.yml
  format: yaml
  label: Convex Environment Variables API
  slug: convex-environment-variables-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/convex/openapi/convex-environment-variables-api-openapi.yml
- filename: convex-custom-roles-api-openapi.yml
  format: yaml
  label: Convex Custom Roles API
  slug: convex-custom-roles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/convex/openapi/convex-custom-roles-api-openapi.yml
- filename: convex-deploy-keys-api-openapi.yml
  format: yaml
  label: Convex Deploy Keys API
  slug: convex-deploy-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/convex/openapi/convex-deploy-keys-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: convex.dev
  spf: true
hosts:
- cert_expires: Sep 23 19:17:07 2026 GMT
  host: www.convex.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 22:53:41 2026 GMT
  host: docs.convex.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 21 23:59:59 2026 GMT
  host: api.convex.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Convex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Convex, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Convex
provider_slug: convex
slug: convex-domain-security
source_filename: convex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.convex.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 19:17:07 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.convex.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 22:53:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.convex.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: convex.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/convex/security/convex-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Backend
- Database
- Functions
- Real-Time
- Reactive
- Serverless
- TypeScript
---
