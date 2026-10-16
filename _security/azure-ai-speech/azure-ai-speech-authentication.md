---
anonymous_access: false
api_key_in: []
api_specs:
- filename: azure-ai-speech-openapi-generated.yml
  format: yaml
  label: Azure AI Speech API
  slug: azure-ai-speech-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-ai-speech/refs/heads/main/openapi/_ae-authored/azure-ai-speech-openapi-generated.yml
auth_types: []
description: Authentication uses JWT bearer tokens sent in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Azure Ai Speech Authentication
name_suffix: Authentication
oauth_flows: []
overview: Azure AI Speech declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Azure AI Speech
provider_slug: azure-ai-speech
scheme_count: 1
schemes:
- evidence: The Microsoft Data sync Framework has built-in support for any authentication provider that uses a Json Web Token (JWT) within a header of the HTTP transaction.
  header: Authorization
  how_to_obtain: Obtain a JWT from Azure AD (Microsoft Entra ID) using the Microsoft Identity platform (MSAL) and include it in the Authorization header as a Bearer token.
  location: header
  name: Bearer
  type: http-bearer
slug: azure-ai-speech-authentication
source_filename: azure-ai-speech-authentication.yml
source_heading: Authentication Profile
source_url: https://learn.microsoft.com/en-us/previous-versions/azure/developer/mobile-apps/azure-mobile-apps/quickstarts/maui/authentication
source_yaml: "generated: '2026-10-13'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://learn.microsoft.com/en-us/previous-versions/azure/developer/mobile-apps/azure-mobile-apps/quickstarts/maui/authentication\nsources:\n- https://learn.microsoft.com/en-us/previous-versions/azure/developer/mobile-apps/azure-mobile-apps/quickstarts/maui/authentication\n- https://learn.microsoft.com/en-us/aspnet/core/security/authentication/?view=aspnetcore-10.0\n- https://learn.microsoft.com/en-us/dotnet/csharp/language-reference/tokens/\n- https://learn.microsoft.com/en-us/adaptive-cards/sdk/rendering-cards/android/getting-started\ndescription: Authentication uses JWT bearer tokens sent in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: The Microsoft Data sync Framework has built-in support for any authentication provider that uses a Json Web Token (JWT) within a header\n    of the HTTP transaction.\n  location: header\n  header: Authorization\n\
  \  how_to_obtain: Obtain a JWT from Azure AD (Microsoft Entra ID) using the Microsoft Identity platform (MSAL) and include it in the Authorization\n    header as a Bearer token.\ndocs: https://learn.microsoft.com/en-us/previous-versions/azure/developer/mobile-apps/azure-mobile-apps/quickstarts/maui/authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/azure-ai-speech/refs/heads/main/authentication/azure-ai-speech-authentication.yml
summary_line: 1 scheme
tags:
- Cloud
- AI
- Speech
- Microsoft
- Service
---
