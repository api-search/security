---
api_key_in: []
api_specs:
- filename: zotgpt-api-openapi.yml
  format: yaml
  label: ZotGPT API (Deprecated)
  slug: api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zotgpt/refs/heads/main/openapi/zotgpt-api-openapi.yml
- filename: zotgpt-gateway-openapi.yml
  format: yaml
  label: ZotGPT (UC Irvine) ZotGPT Gateway
  slug: zotgpt-gateway-openapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zotgpt/refs/heads/main/openapi/zotgpt-gateway-openapi.yml
auth_types: []
description: 'ZotGPT runs two distinct authentication planes. Human access to every interactive product is federated campus SSO — a Shibboleth SAML2 redirect to shib.service.uci.edu, observed live on chat.zotgpt.uci.edu. Machine access is key-based, and the key is always minted only after a human has authenticated with UCInetID: an Azure API Management subscription key for the deprecated API, and a workspace virtual key for the Gateway. There is no anonymous self-service signup on either plane, and there is no public OAuth authorization server.'
kind: authentication
layout: security
method: searched
name: Zotgpt Authentication
name_suffix: Authentication
oauth_flows: []
overview: ZotGPT (UC Irvine) declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: ZotGPT (UC Irvine)
provider_slug: zotgpt
scheme_count: 3
schemes:
- applies_to:
  - https://chat.zotgpt.uci.edu/
  - https://classchat.zotgpt.uci.edu/
  - https://creator.zotgpt.uci.edu/
  - https://app.portkey.ai (Gateway portal sign-in)
  evidence:
    probed: '2026-07-28'
    request: GET https://chat.zotgpt.uci.edu/
    response: HTTP 302 to https://shib.service.uci.edu/idp/profile/SAML2/Redirect/SSO?SAMLRequest=... with an _opensaml_req session cookie (secure, HttpOnly, SameSite=None).
  idp: https://shib.service.uci.edu/idp/profile/SAML2/Redirect/SSO
  name: UCInetID Single Sign-On (Shibboleth SAML 2.0)
  notes: Every end-user surface is behind campus identity. This is the mechanism that makes affiliation-based entitlement possible — the platform knows whether the caller is faculty, staff, a graduate student, or an undergraduate before it decides what they may spend.
  protocol: SAML 2.0
  type: federated-sso
- also_accepted_as: bearer scheme, documented for Anthropic-style clients such as Claude Desktop
  applies_to: https://api.portkey.ai/v1
  controls:
  - per-key spend limits
  - workspace budget enforcement
  - provider selection via x-portkey-provider alias
  handling: UCI documents the virtual key as "treat as a password."
  header: x-portkey-api-key
  in: header
  issued_by: The user, self-service, inside their ZotGPT Gateway workspace after UCInetID sign-in.
  name: Gateway virtual API key
  notes: 'Self-managed key issuance is the structural change from the previous generation: the old API required a ServiceNow ticket per developer, the Gateway does not.'
  scoped_to: workspace
  type: apiKey
- applies_to: https://api.zotgpt.uci.edu/v1
  eligibility: UCI faculty and staff
  end_of_life: '"All remaining Azure API keys disabled" at the end of the three-month migration window.'
  issued_by: Azure API Management developer portal at portal.azureapi.zotgpt.uci.edu, after an approved ServiceNow request (uci.service-now.com KB0013367).
  name: Azure API Management key (deprecated)
  scheme: bearer
  status: deprecated
  type: http
slug: zotgpt-authentication
source_filename: zotgpt-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-28'\nmethod: searched\nsource:\n  - https://zotgpt.uci.edu/services/gateway/\n  - https://zotgpt.uci.edu/services/gateway/clients/\n  - https://zotgpt.uci.edu/services/api/\n  - https://zotgpt.uci.edu/services/chat/\nspecification: API Commons Authentication\nspecificationVersion: '0.1'\nprovider: ZotGPT (UC Irvine)\nproviderId: zotgpt\ndescription: >-\n  ZotGPT runs two distinct authentication planes. Human access to every\n  interactive product is federated campus SSO — a Shibboleth SAML2 redirect to\n  shib.service.uci.edu, observed live on chat.zotgpt.uci.edu. Machine access is\n  key-based, and the key is always minted only after a human has authenticated\n  with UCInetID: an Azure API Management subscription key for the deprecated\n  API, and a workspace virtual key for the Gateway. There is no anonymous\n  self-service signup on either plane, and there is no public OAuth\n  authorization server.\ntags:\n  - Authentication\n  - SSO\n  - SAML\n  - Shibboleth\n\
  \  - API Keys\n  - Identity\nschemes:\n  - name: UCInetID Single Sign-On (Shibboleth SAML 2.0)\n    type: federated-sso\n    protocol: SAML 2.0\n    idp: https://shib.service.uci.edu/idp/profile/SAML2/Redirect/SSO\n    applies_to:\n      - https://chat.zotgpt.uci.edu/\n      - https://classchat.zotgpt.uci.edu/\n      - https://creator.zotgpt.uci.edu/\n      - https://app.portkey.ai (Gateway portal sign-in)\n    evidence:\n      probed: '2026-07-28'\n      request: GET https://chat.zotgpt.uci.edu/\n      response: >-\n        HTTP 302 to\n        https://shib.service.uci.edu/idp/profile/SAML2/Redirect/SSO?SAMLRequest=...\n        with an _opensaml_req session cookie (secure, HttpOnly, SameSite=None).\n    notes: >-\n      Every end-user surface is behind campus identity. This is the mechanism\n      that makes affiliation-based entitlement possible — the platform knows\n      whether the caller is faculty, staff, a graduate student, or an\n      undergraduate before it decides what they\
  \ may spend.\n  - name: Gateway virtual API key\n    type: apiKey\n    in: header\n    header: x-portkey-api-key\n    also_accepted_as: >-\n      bearer scheme, documented for Anthropic-style clients such as Claude\n      Desktop\n    applies_to: https://api.portkey.ai/v1\n    issued_by: >-\n      The user, self-service, inside their ZotGPT Gateway workspace after\n      UCInetID sign-in.\n    scoped_to: workspace\n    controls:\n      - per-key spend limits\n      - workspace budget enforcement\n      - provider selection via x-portkey-provider alias\n    handling: >-\n      UCI documents the virtual key as \"treat as a password.\"\n    notes: >-\n      Self-managed key issuance is the structural change from the previous\n      generation: the old API required a ServiceNow ticket per developer, the\n      Gateway does not.\n  - name: Azure API Management key (deprecated)\n    type: http\n    scheme: bearer\n    applies_to: https://api.zotgpt.uci.edu/v1\n    issued_by: >-\n      Azure\
  \ API Management developer portal at portal.azureapi.zotgpt.uci.edu,\n      after an approved ServiceNow request\n      (uci.service-now.com KB0013367).\n    eligibility: UCI faculty and staff\n    status: deprecated\n    end_of_life: >-\n      \"All remaining Azure API keys disabled\" at the end of the three-month\n      migration window.\nprovider_routing:\n  description: >-\n    The Gateway does not expose upstream vendor credentials to callers. A campus\n    alias is presented instead, and UCI holds the vendor contracts and keys\n    behind it. This is the control point that lets UCI change vendors without\n    changing any campus client code.\n  header: x-portkey-provider\n  aliases_documented:\n    - '@zotgpt-api-bedrock'\n    - '@openai-prod'\n  example_model_slug: '@zotgpt-api-bedrock/us.anthropic.claude-opus-4-7'\noauth:\n  authorization_server: none published\n  probed:\n    - path: /.well-known/oauth-authorization-server\n      host: zotgpt.uci.edu\n      status: 404\ngaps:\n\
  \  - No public, machine-readable authentication reference (no OpenAPI\n    securitySchemes published by UCI, no OIDC discovery document).\n  - No documented key rotation policy or key lifetime for Gateway virtual keys.\n  - No documented scope model — a virtual key is bounded by budget, not by\n    capability.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zotgpt/refs/heads/main/authentication/zotgpt-authentication.yml
summary_line: 3 schemes
tags:
- Authentication
- SSO
- SAML
- Shibboleth
- API Keys
- Identity
---
