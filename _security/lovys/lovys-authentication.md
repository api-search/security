---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Lovys Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lovys secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Lovys
provider_slug: lovys
scheme_count: 1
schemes:
- name: oauth2
  provider: Microsoft Entra ID / Azure Active Directory B2C
  reseller_identification: true
  source: https://docs.lovys.com/signup-oauth
  type: oauth2
slug: lovys-authentication
source_filename: lovys-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.lovys.com/getting-started\ndocs: https://docs.lovys.com/getting-started\nnotes: >-\n  The Lovys Partner API is fronted by Azure API Management. Partner sign-up and\n  authentication are handled through Microsoft Entra ID / Azure Active Directory\n  B2C (see https://docs.lovys.com/signup-oauth), so access is OAuth2-based. The\n  getting-started guide documents an Authentication section plus a \"Reseller\n  Identification\" step, indicating a partner/reseller-scoped OAuth credential in\n  addition to reseller identification headers. The published developer portal is\n  an early-stage scaffold (placeholder bodies), so exact token URLs, flows, and\n  scopes are not yet public; captured here from the documented surfaces only.\nsummary:\n  types:\n  - oauth2\n  identity_provider: Microsoft Entra ID / Azure AD B2C\n  gateway: Azure API Management\nschemes:\n- name: oauth2\n  type: oauth2\n  provider: Microsoft Entra ID\
  \ / Azure Active Directory B2C\n  source: https://docs.lovys.com/signup-oauth\n  reseller_identification: true\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lovys/refs/heads/main/authentication/lovys-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Insurance
- Insurtech
- Embedded Insurance
- Partner API
- Home Insurance
- Pet Insurance
- Smartphone Insurance
- OAuth2
- Azure API Management
---
