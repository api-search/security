---
api_key_in: []
api_specs:
- filename: crowddev-advisories-api-openapi.yml
  format: yaml
  label: Crowd.dev Advisories API
  slug: crowddev-advisories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crowddev/refs/heads/main/openapi/crowddev-advisories-api-openapi.yml
- filename: crowddev-affiliations-api-openapi.yml
  format: yaml
  label: Crowd.dev Affiliations API
  slug: crowddev-affiliations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crowddev/refs/heads/main/openapi/crowddev-affiliations-api-openapi.yml
- filename: crowddev-contacts-api-openapi.yml
  format: yaml
  label: Crowd.dev Contacts API
  slug: crowddev-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crowddev/refs/heads/main/openapi/crowddev-contacts-api-openapi.yml
- filename: crowddev-dashboard-api-openapi.yml
  format: yaml
  label: Crowd.dev Dashboard API
  slug: crowddev-dashboard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crowddev/refs/heads/main/openapi/crowddev-dashboard-api-openapi.yml
- filename: crowddev-maintainer-roles-api-openapi.yml
  format: yaml
  label: Crowd.dev Maintainer Roles API
  slug: crowddev-maintainer-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crowddev/refs/heads/main/openapi/crowddev-maintainer-roles-api-openapi.yml
- filename: crowddev-member-affiliations-api-api-openapi.yml
  format: yaml
  label: Crowd.dev Member Affiliations API API
  slug: crowddev-member-affiliations-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crowddev/refs/heads/main/openapi/crowddev-member-affiliations-api-api-openapi.yml
- filename: crowddev-member-identities-api-openapi.yml
  format: yaml
  label: Crowd.dev Member Identities API
  slug: crowddev-member-identities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crowddev/refs/heads/main/openapi/crowddev-member-identities-api-openapi.yml
- filename: crowddev-member-organizations-api-api-openapi.yml
  format: yaml
  label: Crowd.dev Member Organizations API API
  slug: crowddev-member-organizations-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crowddev/refs/heads/main/openapi/crowddev-member-organizations-api-api-openapi.yml
- filename: crowddev-members-api-openapi.yml
  format: yaml
  label: Crowd.dev Members API
  slug: crowddev-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crowddev/refs/heads/main/openapi/crowddev-members-api-openapi.yml
- filename: crowddev-organizations-api-openapi.yml
  format: yaml
  label: Crowd.dev Organizations API
  slug: crowddev-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crowddev/refs/heads/main/openapi/crowddev-organizations-api-openapi.yml
- filename: crowddev-packages-api-openapi.yml
  format: yaml
  label: Crowd.dev Packages API
  slug: crowddev-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crowddev/refs/heads/main/openapi/crowddev-packages-api-openapi.yml
- filename: crowddev-project-affiliations-api-openapi.yml
  format: yaml
  label: Crowd.dev Project Affiliations API
  slug: crowddev-project-affiliations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crowddev/refs/heads/main/openapi/crowddev-project-affiliations-api-openapi.yml
- filename: crowddev-stewardship-actions-api-openapi.yml
  format: yaml
  label: Crowd.dev Stewardship Actions API
  slug: crowddev-stewardship-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crowddev/refs/heads/main/openapi/crowddev-stewardship-actions-api-openapi.yml
- filename: crowddev-stewardship-api-openapi.yml
  format: yaml
  label: Crowd.dev Stewardship API
  slug: crowddev-stewardship-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crowddev/refs/heads/main/openapi/crowddev-stewardship-api-openapi.yml
- filename: crowddev-stewardships-api-openapi.yml
  format: yaml
  label: Crowd.dev Stewardships API
  slug: crowddev-stewardships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crowddev/refs/heads/main/openapi/crowddev-stewardships-api-openapi.yml
- filename: crowddev-work-experiences-api-openapi.yml
  format: yaml
  label: Crowd.dev Work Experiences API
  slug: crowddev-work-experiences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crowddev/refs/heads/main/openapi/crowddev-work-experiences-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Crowddev Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Crowd.dev secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Crowd.dev
provider_slug: crowddev
scheme_count: 2
schemes:
- description: 'Auth0 machine-to-machine client-credentials flow. Akrites exchanges its client ID/secret with Auth0 for a JWT and sends it as `Authorization: Bearer <token>`; CDP only verifies the resulting token.'
  flows:
  - flow: clientCredentials
    scopes: 3
    tokenUrl: https://linuxfoundation.auth0.com/oauth/token
  name: M2MBearer
  sources:
  - openapi/crowddev-cdp-akrites-external-openapi.yml
  - openapi/crowddev-cdp-public-openapi.yml
  type: oauth2
- bearerFormat: JWT
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/crowddev-cdp-akrites-openapi.yml
  - openapi/crowddev-cdp-ossprey-openapi.yml
  - openapi/crowddev-cdp-packages-openapi.yml
  - openapi/crowddev-cdp-public-openapi.yml
  - openapi/crowddev-cdp-stewardships-openapi.yml
  - openapi/crowddev-cm-id-openapi.yml
  type: http
slug: crowddev-authentication
source_filename: crowddev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/crowddev-cdp-akrites-external-openapi.yml, openapi/crowddev-cdp-akrites-openapi.yml,\n  openapi/crowddev-cdp-ossprey-openapi.yml, openapi/crowddev-cdp-packages-openapi.yml, openapi/crowddev-cdp-public-openapi.yml,\n  openapi/crowddev-cdp-stewardships-openapi.yml, openapi/crowddev-cm-id-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: M2MBearer\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://linuxfoundation.auth0.com/oauth/token\n    scopes: 3\n  description: 'Auth0 machine-to-machine client-credentials flow. Akrites exchanges its client\n    ID/secret with Auth0 for a JWT and sends it as `Authorization: Bearer <token>`; CDP only\n    verifies the resulting token.'\n  sources:\n  - openapi/crowddev-cdp-akrites-external-openapi.yml\n  - openapi/crowddev-cdp-public-openapi.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n\
  \  bearerFormat: JWT\n  sources:\n  - openapi/crowddev-cdp-akrites-openapi.yml\n  - openapi/crowddev-cdp-ossprey-openapi.yml\n  - openapi/crowddev-cdp-packages-openapi.yml\n  - openapi/crowddev-cdp-public-openapi.yml\n  - openapi/crowddev-cdp-stewardships-openapi.yml\n  - openapi/crowddev-cm-id-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crowddev/refs/heads/main/authentication/crowddev-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Community
- Developer Relations
- Developer Data Platform
- Identity Resolution
- Open Source
- Community Data Platform
- Open Source Intelligence
---
