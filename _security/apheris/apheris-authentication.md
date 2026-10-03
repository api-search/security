---
anonymous_access: false
api_key_in: []
api_specs:
- filename: apheris-apheris-api-api-openapi.yml
  format: yaml
  label: Apheris Apheris API
  slug: apheris-apheris-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apheris/refs/heads/main/openapi/apheris-apheris-api-api-openapi.yml
- filename: apheris-health-api-openapi.yml
  format: yaml
  label: Apheris Health API
  slug: apheris-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apheris/refs/heads/main/openapi/apheris-health-api-openapi.yml
- filename: apheris-predict-async-api-openapi.yml
  format: yaml
  label: Apheris Predict Async API
  slug: apheris-predict-async-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apheris/refs/heads/main/openapi/apheris-predict-async-api-openapi.yml
- filename: apheris-results-api-openapi.yml
  format: yaml
  label: Apheris Results API
  slug: apheris-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apheris/refs/heads/main/openapi/apheris-results-api-openapi.yml
- filename: apheris-schema-api-openapi.yml
  format: yaml
  label: Apheris Schema API
  slug: apheris-schema-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apheris/refs/heads/main/openapi/apheris-schema-api-openapi.yml
- filename: apheris-ticket-api-openapi.yml
  format: yaml
  label: Apheris Ticket API
  slug: apheris-ticket-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apheris/refs/heads/main/openapi/apheris-ticket-api-openapi.yml
- filename: apheris-weights-api-openapi.yml
  format: yaml
  label: Apheris Weights API
  slug: apheris-weights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apheris/refs/heads/main/openapi/apheris-weights-api-openapi.yml
auth_types: []
description: Authentication schemes for Apheris Hub
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Apheris Authentication
name_suffix: Authentication
oauth_flows: []
overview: Apheris declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Apheris
provider_slug: apheris
scheme_count: 1
schemes:
- evidence: This guide provides the steps required to configure your OAuth 2.0 / OpenID Connect (OIDC) identity provider so the Apheris Hub can validate JWTs and support multi-user deployments.
  flows:
  - authorization_code
  how_to_obtain: Configure an OIDC‑compatible identity provider (e.g., Auth0, Microsoft Entra, ForgeRock, Dex) and set the required hub.auth fields (domain, audience, clientId, etc.) in the Hub configuration.
  name: oidc
  type: oauth2
slug: apheris-authentication
source_filename: apheris-authentication.yml
source_heading: Authentication Profile
source_url: https://www.apheris.com/docs/hub/authentication-setup.html
source_yaml: "generated: '2026-09-25'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.apheris.com/docs/hub/authentication-setup.html\nsources:\n- https://www.apheris.com/docs/hub/authentication-setup.html\n- https://www.apheris.com/docs/hub/nim-msa-server-setup.html\ndescription: Authentication schemes for Apheris Hub\nschemes:\n- type: oauth2\n  name: oidc\n  evidence: This guide provides the steps required to configure your OAuth 2.0 / OpenID Connect (OIDC) identity provider so the Apheris Hub can\n    validate JWTs and support multi-user deployments.\n  flows:\n  - authorization_code\n  how_to_obtain: Configure an OIDC‑compatible identity provider (e.g., Auth0, Microsoft Entra, ForgeRock, Dex) and set the required hub.auth fields\n    (domain, audience, clientId, etc.) in the Hub configuration.\ndocs: https://www.apheris.com/docs/hub/authentication-setup.html\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apheris/refs/heads/main/authentication/apheris-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Artificial Intelligence
- Drug Discovery
- Federated Learning
- Biotechnology
---
