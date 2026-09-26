---
anonymous_access: false
api_key_in: []
api_specs:
- filename: apheris-openapi-generated.yml
  format: yaml
  label: Apheris API
  slug: apheris-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apheris/refs/heads/main/openapi/_ae-authored/apheris-openapi-generated.yml
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
- AI
- DrugDiscovery
- FederatedLearning
- Biotechnology
---
