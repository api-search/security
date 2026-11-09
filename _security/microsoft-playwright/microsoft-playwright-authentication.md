---
anonymous_access: false
api_key_in: []
api_specs:
- filename: microsoft-playwright-accountquotas-api-openapi.yml
  format: yaml
  label: Microsoft Playwright Account Quotas API
  slug: microsoft-playwright-accountquotas-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-playwright/openapi/microsoft-playwright-accountquotas-api-openapi.yml
- filename: microsoft-playwright-accounts-api-openapi.yml
  format: yaml
  label: Microsoft Playwright Accounts API
  slug: microsoft-playwright-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-playwright/openapi/microsoft-playwright-accounts-api-openapi.yml
- filename: microsoft-playwright-operations-api-openapi.yml
  format: yaml
  label: Microsoft Playwright Operations API
  slug: microsoft-playwright-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-playwright/openapi/microsoft-playwright-operations-api-openapi.yml
- filename: microsoft-playwright-quotas-api-openapi.yml
  format: yaml
  label: Microsoft Playwright Quotas API
  slug: microsoft-playwright-quotas-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-playwright/openapi/microsoft-playwright-quotas-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Microsoft Playwright Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
overview: Microsoft Playwright secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and implicit flow(s).
provider_name: Microsoft Playwright
provider_slug: microsoft-playwright
scheme_count: 2
schemes:
- flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
    scopes: 1
  name: OAuth2Auth
  sources:
  - openapi/microsoft-playwright-authmanager-openapi.yml
  - openapi/microsoft-playwright-management-openapi.yml
  type: oauth2
- flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://login.microsoftonline.com/common/v2.0/oauth2/token
  name: OAuth2Auth_
  sources:
  - openapi/microsoft-playwright-authmanager-openapi.yml
  type: oauth2
slug: microsoft-playwright-authentication
source_filename: microsoft-playwright-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/microsoft-playwright-authmanager-openapi.yml, openapi/microsoft-playwright-management-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - implicit\nschemes:\n- name: OAuth2Auth\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n    scopes: 1\n  sources:\n  - openapi/microsoft-playwright-authmanager-openapi.yml\n  - openapi/microsoft-playwright-management-openapi.yml\n- name: OAuth2Auth_\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n    tokenUrl: https://login.microsoftonline.com/common/v2.0/oauth2/token\n    scopes: 1\n  sources:\n  - openapi/microsoft-playwright-authmanager-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/microsoft-playwright/authentication/microsoft-playwright-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Browser Automation
- End-to-End Testing
- Microsoft
- Testing
- Open Source
- MCP
- Microsoft Azure
---
