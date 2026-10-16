---
anonymous_access: false
api_key_in: []
api_specs:
- filename: azure-ai-search-openapi-generated.yml
  format: yaml
  label: Azure AI Search API
  slug: azure-ai-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-ai-search/refs/heads/main/openapi/_ae-authored/azure-ai-search-openapi-generated.yml
auth_types: []
description: Authentication methods for Azure AI Search as documented.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Azure Ai Search Authentication
name_suffix: Authentication
oauth_flows: []
overview: Azure AI Search declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Azure AI Search
provider_slug: azure-ai-search
scheme_count: 2
schemes:
- evidence: Set an admin key in the request header. You can't pass admin keys on the URI or in the body of the request.
  header: api-key
  how_to_obtain: Admin and query keys are generated when the search service is created and can be retrieved via the Azure portal, REST API, Azure CLI, PowerShell, or SDKs.
  location: header
  name: API key
  type: apiKey
- authorize_url: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/authorize
  evidence: builder.Services.AddAuthentication(JwtBearerDefaults.AuthenticationScheme).AddMicrosoftIdentityWebApi(builder.Configuration);
  header: Authorization
  how_to_obtain: Register an application in Azure AD, define a scope (e.g., access_as_user), and acquire a JWT via the OAuth 2.0 client credentials or authorization code flow using MSAL.
  location: header
  name: Azure AD (Microsoft Entra ID) JWT bearer
  scopes:
  - api://<client-id>/access_as_user
  token_url: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token
  type: oauth2
slug: azure-ai-search-authentication
source_filename: azure-ai-search-authentication.yml
source_heading: Authentication Profile
source_url: https://learn.microsoft.com/en-us/previous-versions/azure/developer/mobile-apps/azure-mobile-apps/quickstarts/maui/authentication
source_yaml: "generated: '2026-10-13'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://learn.microsoft.com/en-us/previous-versions/azure/developer/mobile-apps/azure-mobile-apps/quickstarts/maui/authentication\nsources:\n- https://learn.microsoft.com/en-us/previous-versions/azure/developer/mobile-apps/azure-mobile-apps/quickstarts/maui/authentication\n- https://learn.microsoft.com/en-us/aspnet/core/security/authentication/?view=aspnetcore-10.0\n- https://learn.microsoft.com/en-us/azure/search/search-security-api-keys\n- https://learn.microsoft.com/en-us/azure/search/search-security-rbac\ndescription: Authentication methods for Azure AI Search as documented.\nschemes:\n- type: apiKey\n  name: API key\n  evidence: Set an admin key in the request header. You can't pass admin keys on the URI or in the body of the request.\n  location: header\n  header: api-key\n  how_to_obtain: Admin and query keys are generated when the search service is created and can be retrieved\
  \ via the Azure portal, REST API, Azure\n    CLI, PowerShell, or SDKs.\n- type: oauth2\n  name: Azure AD (Microsoft Entra ID) JWT bearer\n  evidence: builder.Services.AddAuthentication(JwtBearerDefaults.AuthenticationScheme).AddMicrosoftIdentityWebApi(builder.Configuration);\n  location: header\n  header: Authorization\n  token_url: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token\n  authorize_url: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/authorize\n  scopes:\n  - api://<client-id>/access_as_user\n  how_to_obtain: Register an application in Azure AD, define a scope (e.g., access_as_user), and acquire a JWT via the OAuth 2.0 client credentials\n    or authorization code flow using MSAL.\ndocs: https://learn.microsoft.com/en-us/previous-versions/azure/developer/mobile-apps/azure-mobile-apps/quickstarts/maui/authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/azure-ai-search/refs/heads/main/authentication/azure-ai-search-authentication.yml
summary_line: 2 schemes
tags:
- AI
- Search
- Azure
- Cloud
- Service
---
