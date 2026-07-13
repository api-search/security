---
api_key_in: []
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Vercel REST API
  slug: vercel-rest-api
  spec_type: OpenAPI
  url: https://openapi.vercel.sh/
- filename: openapi.yaml
  format: yaml
  label: Netlify API
  slug: netlify-api
  spec_type: OpenAPI
  url: https://open-api.netlify.com/
- filename: openapi.yaml
  format: yaml
  label: Cloudflare API
  slug: cloudflare-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/cloudflare/api-schemas/main/openapi.yaml
- filename: api-docs
  format: yaml
  label: Heroku Platform API
  slug: heroku-platform-api
  spec_type: OpenAPI
  url: https://devcenter.heroku.com/api-docs
- filename: openapi.yaml
  format: yaml
  label: Fly.io Machines API
  slug: flyio-machines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/superfly/fly-openapi/refs/heads/main/openapi.yaml
- filename: openapi.yaml
  format: yaml
  label: Render API
  slug: render-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/renderinc/openapi-specs/main/openapi.yaml
- filename: openapi.json
  format: json
  label: Northflank API
  slug: northflank-api
  spec_type: OpenAPI
  url: https://api.northflank.com/v1/openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Scalable Platforms Authentication
name_suffix: Authentication
oauth_flows: []
overview: Scalable Platforms secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Scalable Platforms
provider_slug: scalable-platforms
scheme_count: 1
schemes:
- bearerFormat: VercelToken
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/scalable-platforms-openapi.yml
  type: http
slug: scalable-platforms-authentication
source_filename: scalable-platforms-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/scalable-platforms-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: VercelToken\n  sources:\n  - openapi/scalable-platforms-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scalable-platforms/refs/heads/main/authentication/scalable-platforms-authentication.yml
summary_line: http · 1 scheme
tags:
- Cloud Infrastructure
- Deployment
- Developer Experience
- DevOps
- PaaS
- Platform
- Scalability
- Serverless
---
