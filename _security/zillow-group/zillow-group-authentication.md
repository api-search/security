---
api_key_in: []
auth_types: []
description: 'Authentication profile for the Zillow Group API surface, read from the per-API fact panels Zillow Group publishes on its own developer portal. There is no single Zillow Group auth model: the portal is a directory over four separately-operated platforms, each with its own scheme. No securityScheme could be derived from a specification, because Zillow Group publishes no OpenAPI, Swagger, GraphQL SDL or AsyncAPI document on any host.'
kind: authentication
layout: security
method: searched
name: Zillow Group Authentication
name_suffix: Authentication
oauth_flows: []
overview: Zillow Group declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Zillow Group
provider_slug: zillow-group
scheme_count: 4
schemes:
- applies_to:
  - Zestimate API
  - Public Records API
  - MLS Listings API
  - Reviews API
  - Zillow Agent Reviews API
  docs: https://bridgedataoutput.com/docs/platform
  evidence: 'Zillow Group''s own API pages state "Password and access token authentication" and route access-token issuance to the Bridge dashboard: "Your access tokens can also be found on your Bridge Dashboard under Data Access > API Access Tokens."'
  id: bridge-bearer-token
  label: Bridge access token (server token)
  note: Served by Bridge Interactive, a Zillow Group company; Zillow Group's own developer portal names bridgedataoutput.com as the reference for these APIs, which is why a different domain appears here.
  onboarding: Register at https://bridgedataoutput.com/register, then API Access > Request Data Access > Zillow Group Datasets > agree to the Zillow Data Terms of Use > apply for the dataset.
  scheme: bearer
  type: http
- applies_to:
  - Rate Cloud API
  - Prospect Sync API
  - Prospect Trigger API
  - Lead Posting API
  - LOS Plug-In Integration API
  docs: https://www.zillowgroup.com/developers/mortgage/
  evidence: Every Mortech-powered mortgage API page publishes the same authentication value, "Third Party Name, License Key", with HTTP POST requests and XML responses.
  id: mortech-license-key
  in: body
  label: Third Party Name + License Key
  onboarding: Request-access form; agreement type is "Partner/MSA".
  type: apiKey
- applies_to:
  - Transaction Management API
  authorization_url: https://auth.dotloop.com/oauth/authorize
  bearer_header: 'Authorization: Bearer <access token>'
  client_registration: http://info.dotloop.com/developers
  docs: https://dotloop.github.io/public-api/
  evidence: Zillow Group's Transaction Management page states "OAuth 2.0 / 3-legged OAuth"; the linked dotloop Public API v2 guide documents the authorize/token/revoke endpoints and a Basic-auth client credential on the /token call.
  id: dotloop-oauth2
  label: OAuth 2.0 three-legged authorization code
  note: Served by dotloop, a Zillow Group company, and profiled in depth in its own repo (all/dotloop). Recorded here because Zillow Group lists it as one of its own developer APIs at https://www.zillowgroup.com/developers/api/transactions/transaction-management/.
  revocation_url: https://auth.dotloop.com/oauth/token/revoke
  token_lifetime: 12 hours (refresh token required thereafter)
  token_url: https://auth.dotloop.com/oauth/token
  type: oauth2
- applies_to:
  - Rentals Lead API
  docs: https://s3.amazonaws.com/files.hotpads.com/+guides/Lead+API+Guide.pdf
  evidence: The Lead API delivers URL-encoded HTTP POST callbacks to a customer-supplied webhook endpoint. Zillow Group's page documents no signing, shared secret or mutual TLS for those callbacks, and states "we are unable to make changes to our API fields or form".
  gap: true
  id: rentals-webhook-callback
  label: No inbound authentication documented
  type: none
slug: zillow-group-authentication
source_filename: zillow-group-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-28'\nmethod: searched\nsource: https://www.zillowgroup.com/developers/\ndescription: >-\n  Authentication profile for the Zillow Group API surface, read from the per-API fact panels\n  Zillow Group publishes on its own developer portal. There is no single Zillow Group auth\n  model: the portal is a directory over four separately-operated platforms, each with its own\n  scheme. No securityScheme could be derived from a specification, because Zillow Group\n  publishes no OpenAPI, Swagger, GraphQL SDL or AsyncAPI document on any host.\nderived_from_spec: false\nschemes:\n  - id: bridge-bearer-token\n    type: http\n    scheme: bearer\n    label: Bridge access token (server token)\n    applies_to:\n      - Zestimate API\n      - Public Records API\n      - MLS Listings API\n      - Reviews API\n      - Zillow Agent Reviews API\n    docs: https://bridgedataoutput.com/docs/platform\n    evidence: >-\n      Zillow Group's own API pages state \"Password and access\
  \ token authentication\" and route\n      access-token issuance to the Bridge dashboard: \"Your access tokens can also be found on\n      your Bridge Dashboard under Data Access > API Access Tokens.\"\n    onboarding: >-\n      Register at https://bridgedataoutput.com/register, then API Access > Request Data Access\n      > Zillow Group Datasets > agree to the Zillow Data Terms of Use > apply for the dataset.\n    note: >-\n      Served by Bridge Interactive, a Zillow Group company; Zillow Group's own developer portal\n      names bridgedataoutput.com as the reference for these APIs, which is why a different\n      domain appears here.\n  - id: mortech-license-key\n    type: apiKey\n    in: body\n    label: Third Party Name + License Key\n    applies_to:\n      - Rate Cloud API\n      - Prospect Sync API\n      - Prospect Trigger API\n      - Lead Posting API\n      - LOS Plug-In Integration API\n    docs: https://www.zillowgroup.com/developers/mortgage/\n    evidence: >-\n      Every\
  \ Mortech-powered mortgage API page publishes the same authentication value,\n      \"Third Party Name, License Key\", with HTTP POST requests and XML responses.\n    onboarding: Request-access form; agreement type is \"Partner/MSA\".\n  - id: dotloop-oauth2\n    type: oauth2\n    label: OAuth 2.0 three-legged authorization code\n    applies_to:\n      - Transaction Management API\n    docs: https://dotloop.github.io/public-api/\n    authorization_url: https://auth.dotloop.com/oauth/authorize\n    token_url: https://auth.dotloop.com/oauth/token\n    revocation_url: https://auth.dotloop.com/oauth/token/revoke\n    token_lifetime: 12 hours (refresh token required thereafter)\n    bearer_header: 'Authorization: Bearer <access token>'\n    client_registration: http://info.dotloop.com/developers\n    evidence: >-\n      Zillow Group's Transaction Management page states \"OAuth 2.0 / 3-legged OAuth\"; the\n      linked dotloop Public API v2 guide documents the authorize/token/revoke endpoints\
  \ and a\n      Basic-auth client credential on the /token call.\n    note: >-\n      Served by dotloop, a Zillow Group company, and profiled in depth in its own repo\n      (all/dotloop). Recorded here because Zillow Group lists it as one of its own developer\n      APIs at https://www.zillowgroup.com/developers/api/transactions/transaction-management/.\n  - id: rentals-webhook-callback\n    type: none\n    label: No inbound authentication documented\n    applies_to:\n      - Rentals Lead API\n    docs: https://s3.amazonaws.com/files.hotpads.com/+guides/Lead+API+Guide.pdf\n    evidence: >-\n      The Lead API delivers URL-encoded HTTP POST callbacks to a customer-supplied webhook\n      endpoint. Zillow Group's page documents no signing, shared secret or mutual TLS for\n      those callbacks, and states \"we are unable to make changes to our API fields or form\".\n    gap: true\nunauthenticated_surfaces:\n  - name: Zillow Research data (Real Estate Metrics, Neighborhood Data)\n    url:\
  \ https://www.zillow.com/research/data/\n    style: CSV download, no key\n    note: Free for public use; a download portal rather than a keyed API.\ngaps:\n  - No OAuth scope reference is published at the Zillow Group level; only the dotloop subsidiary documents scopes.\n  - No API key rotation, expiry or revocation policy is published for the Bridge or Mortech schemes.\n  - Rentals Lead API webhook deliveries carry no documented signature, so a receiver cannot verify origin.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zillow-group/refs/heads/main/authentication/zillow-group-authentication.yml
summary_line: 4 schemes
tags:
- Real-Estate
- Property-Data
- MLS
- Mortgage
- Rentals
- Valuation
- Housing-Data
- Transaction-Management
---
