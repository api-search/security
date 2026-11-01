---
anonymous_access: false
api_key_in: []
api_specs:
- filename: wevo-wevo-api-api-openapi.yml
  format: yaml
  label: Wevo API
  slug: wevo-api-2
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wevo/openapi/wevo-wevo-api-api-openapi.yml
- filename: wevo-openapi-generated.yml
  format: yaml
  label: Wevo API
  slug: wevo-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wevo/openapi/_ae-authored/wevo-openapi-generated.yml
auth_types: []
description: Authentication schemes for Wevo as documented on the provided pages.
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Wevo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Wevo declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Wevo
provider_slug: wevo
scheme_count: 3
schemes:
- evidence: The Jitterbit OAuth - Google - Service Account plugin is used to authenticate with Google's implementation of OAuth 2 for Google service accounts.
  name: Google Service Account
  type: oauth2
- evidence: When 3-legged OAuth 2.0 is being used, the browser redirects to the native login interface for Microsoft Entra ID. Provide your credentials to authenticate with Microsoft Entra ID.
  name: Microsoft Entra ID 3-legged
  type: oauth2
- evidence: The browser redirects to the native login interface for Google. Provide your credentials to authenticate with Google.
  name: Google 3-legged
  type: oauth2
slug: wevo-authentication
source_filename: wevo-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.jitterbit.com/agent/plugins/oauth-google-service-account/
source_yaml: "generated: '2026-10-21'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.jitterbit.com/agent/plugins/oauth-google-service-account/\nsources:\n- https://docs.jitterbit.com/agent/plugins/oauth-google-service-account/\n- https://docs.jitterbit.com/api-manager/api-manager-reference/api-identity-provider-configuration/azure-ad-2-legged-oauth-2-0-api-security-profile/\n- https://docs.jitterbit.com/api-manager/api-manager-reference/api-identity-provider-configuration/azure-ad-3-legged-oauth-2-0-api-security-profile/\n- https://docs.jitterbit.com/api-manager/api-manager-reference/api-identity-provider-configuration/google-3-legged-oauth-2-0-api-security-profile/\ndescription: Authentication schemes for Wevo as documented on the provided pages.\nschemes:\n- type: oauth2\n  name: Google Service Account\n  evidence: The Jitterbit OAuth - Google - Service Account plugin is used to authenticate with Google's implementation of OAuth 2 for Google service\n\
  \    accounts.\n- type: oauth2\n  name: Microsoft Entra ID 3-legged\n  evidence: When 3-legged OAuth 2.0 is being used, the browser redirects to the native login interface for Microsoft Entra ID. Provide your credentials\n    to authenticate with Microsoft Entra ID.\n- type: oauth2\n  name: Google 3-legged\n  evidence: The browser redirects to the native login interface for Google. Provide your credentials to authenticate with Google.\ndocs: https://docs.jitterbit.com/agent/plugins/oauth-google-service-account/\nnote: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/wevo/authentication/wevo-authentication.yml
summary_line: 3 schemes
tags:
- Integration
- Automation
- iPaaS
- API Management
- Low-code
- Artificial Intelligence
- EDI
---
