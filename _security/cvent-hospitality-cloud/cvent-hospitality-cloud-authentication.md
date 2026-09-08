---
anonymous_access: false
api_key_in: []
api_specs:
- filename: cvent-hospitality-cloud-housing-openapi.yml
  format: yaml
  label: Cvent Passkey RegLink API
  slug: passkey-reglink
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvent-hospitality-cloud/refs/heads/main/openapi/cvent-hospitality-cloud-housing-openapi.yml
- filename: cvent-hospitality-cloud-authentication-openapi.yml
  format: yaml
  label: Cvent Platform REST API (Hospitality)
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvent-hospitality-cloud/refs/heads/main/openapi/cvent-hospitality-cloud-authentication-openapi.yml
- filename: cvent-hospitality-cloud-rfp-management-openapi.yml
  format: yaml
  label: Cvent RFP Management API
  slug: rfp-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvent-hospitality-cloud/refs/heads/main/openapi/cvent-hospitality-cloud-rfp-management-openapi.yml
- filename: cvent-hospitality-cloud-rfp-requirements-openapi.yml
  format: yaml
  label: Cvent RFP Requirements API
  slug: rfp-requirements
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvent-hospitality-cloud/refs/heads/main/openapi/cvent-hospitality-cloud-rfp-requirements-openapi.yml
- filename: cvent-hospitality-cloud-rfp-suppliers-openapi.yml
  format: yaml
  label: Cvent RFP Suppliers API
  slug: rfp-suppliers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvent-hospitality-cloud/refs/heads/main/openapi/cvent-hospitality-cloud-rfp-suppliers-openapi.yml
- filename: cvent-hospitality-cloud-rfp-additional-details-openapi.yml
  format: yaml
  label: Cvent RFP Additional Details API
  slug: rfp-additional-details
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvent-hospitality-cloud/refs/heads/main/openapi/cvent-hospitality-cloud-rfp-additional-details-openapi.yml
- filename: cvent-hospitality-cloud-proposal-drafts-openapi.yml
  format: yaml
  label: Cvent Proposal Draft API
  slug: proposal-drafts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvent-hospitality-cloud/refs/heads/main/openapi/cvent-hospitality-cloud-proposal-drafts-openapi.yml
- filename: cvent-hospitality-cloud-venue-profiles-openapi.yml
  format: yaml
  label: Cvent Venue Profiles API
  slug: venue-profiles
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvent-hospitality-cloud/refs/heads/main/openapi/cvent-hospitality-cloud-venue-profiles-openapi.yml
- filename: cvent-hospitality-cloud-venue-meeting-rooms-openapi.yml
  format: yaml
  label: Cvent Venue Meeting Rooms API
  slug: venue-meeting-rooms
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvent-hospitality-cloud/refs/heads/main/openapi/cvent-hospitality-cloud-venue-meeting-rooms-openapi.yml
- filename: cvent-hospitality-cloud-meeting-requests-openapi.yml
  format: yaml
  label: Cvent Meeting Request API
  slug: meeting-requests
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvent-hospitality-cloud/refs/heads/main/openapi/cvent-hospitality-cloud-meeting-requests-openapi.yml
- filename: cvent-hospitality-cloud-travel-rfps-openapi.yml
  format: yaml
  label: Cvent Travel RFPs API
  slug: travel-rfps
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvent-hospitality-cloud/refs/heads/main/openapi/cvent-hospitality-cloud-travel-rfps-openapi.yml
- filename: cvent-hospitality-cloud-travel-suppliers-openapi.yml
  format: yaml
  label: Cvent Travel Suppliers API
  slug: travel-suppliers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvent-hospitality-cloud/refs/heads/main/openapi/cvent-hospitality-cloud-travel-suppliers-openapi.yml
- filename: cvent-hospitality-cloud-travel-accounts-openapi.yml
  format: yaml
  label: Cvent Travel Accounts API
  slug: travel-accounts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvent-hospitality-cloud/refs/heads/main/openapi/cvent-hospitality-cloud-travel-accounts-openapi.yml
- filename: cvent-hospitality-cloud-event-travel-openapi.yml
  format: yaml
  label: Cvent Event Travel API
  slug: event-travel
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvent-hospitality-cloud/refs/heads/main/openapi/cvent-hospitality-cloud-event-travel-openapi.yml
- filename: cvent-hospitality-cloud-signatures-openapi.yml
  format: yaml
  label: Cvent Signatures API
  slug: signatures
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvent-hospitality-cloud/refs/heads/main/openapi/cvent-hospitality-cloud-signatures-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Cvent Hospitality Cloud Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Cvent Hospitality Cloud secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Cvent Hospitality Cloud
provider_slug: cvent-hospitality-cloud
scheme_count: 2
schemes:
- description: OAuth2 Client Credentials Flow.
  flows:
  - flow: clientCredentials
    scopes: 238
    tokenUrl: https://api-platform.cvent.com/ea/oauth2/token
  name: OAuth2.clientCredentials
  sources:
  - openapi/cvent-hospitality-cloud-authentication-openapi.yml
  - openapi/cvent-hospitality-cloud-event-travel-openapi.yml
  - openapi/cvent-hospitality-cloud-housing-hotels-openapi.yml
  - openapi/cvent-hospitality-cloud-housing-openapi.yml
  - openapi/cvent-hospitality-cloud-meeting-requests-openapi.yml
  - openapi/cvent-hospitality-cloud-proposal-drafts-openapi.yml
  - openapi/cvent-hospitality-cloud-rfp-additional-details-openapi.yml
  - openapi/cvent-hospitality-cloud-rfp-management-openapi.yml
  - openapi/cvent-hospitality-cloud-rfp-requirements-openapi.yml
  - openapi/cvent-hospitality-cloud-rfp-suppliers-openapi.yml
  - openapi/cvent-hospitality-cloud-signatures-openapi.yml
  - openapi/cvent-hospitality-cloud-travel-accounts-openapi.yml
  - openapi/cvent-hospitality-cloud-travel-rfps-openapi.yml
  - openapi/cvent-hospitality-cloud-travel-suppliers-openapi.yml
  - openapi/cvent-hospitality-cloud-venue-meeting-rooms-openapi.yml
  - openapi/cvent-hospitality-cloud-venue-profiles-openapi.yml
  type: oauth2
- description: OAuth2 Authorization Code Flow.
  flows:
  - authorizationUrl: https://api-platform.cvent.com/ea/oauth2/authorize
    flow: authorizationCode
    scopes: 208
    tokenUrl: https://api-platform.cvent.com/ea/oauth2/token
  name: OAuth2.authorizationCode
  sources:
  - openapi/cvent-hospitality-cloud-authentication-openapi.yml
  - openapi/cvent-hospitality-cloud-event-travel-openapi.yml
  - openapi/cvent-hospitality-cloud-meeting-requests-openapi.yml
  - openapi/cvent-hospitality-cloud-rfp-additional-details-openapi.yml
  - openapi/cvent-hospitality-cloud-rfp-management-openapi.yml
  - openapi/cvent-hospitality-cloud-rfp-requirements-openapi.yml
  - openapi/cvent-hospitality-cloud-rfp-suppliers-openapi.yml
  - openapi/cvent-hospitality-cloud-signatures-openapi.yml
  - openapi/cvent-hospitality-cloud-travel-rfps-openapi.yml
  - openapi/cvent-hospitality-cloud-venue-meeting-rooms-openapi.yml
  - openapi/cvent-hospitality-cloud-venue-profiles-openapi.yml
  type: oauth2
slug: cvent-hospitality-cloud-authentication
source_filename: cvent-hospitality-cloud-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: searched\ndocs:\n  - https://developers.cvent.com/docs/rest-api/reference/reference\n  - https://developers.cvent.com/docs/rest-api/tutorials/developer-quickstart\n  - https://developers.cvent.com/docs/rest-api/explanation/concepts\nnote: >-\n  Read from the securitySchemes block of the contract Cvent publishes at\n  https://developers.cvent.com/documentation and cross-checked against the developer portal. Every\n  hospitality operation is OAuth 2.0 bearer-protected: 'Authorization: Bearer {accessToken}', tokens\n  valid for 60 minutes, minted at https://api-platform.cvent.com/ea/oauth2/token. Machine-to-machine\n  integrations use client credentials and the call is attributed to the application; web applications use\n  the authorization code flow and the call is attributed to the authenticating Cvent administrator, who\n  must be both an admin and a registered developer.\n  Two additional schemes in the contract, CallbackApiKeyAuth and CallbackBasicAuth,\
  \ are INBOUND — they\n  describe how Cvent authenticates itself to a subscriber's webhook endpoint, not how a client\n  authenticates to Cvent.\n  The legacy SOAP API does NOT use OAuth: it exchanges credentials for a session ticket via its own Login\n  call (see wsdl/cvent-hospitality-cloud-soap-v200611.yml).\ntoken_lifetime: 60 minutes\nscope_count: 238\nsource: openapi/cvent-hospitality-cloud-authentication-openapi.yml, openapi/cvent-hospitality-cloud-event-travel-openapi.yml,\n  openapi/cvent-hospitality-cloud-housing-hotels-openapi.yml, openapi/cvent-hospitality-cloud-housing-openapi.yml,\n  openapi/cvent-hospitality-cloud-meeting-requests-openapi.yml, openapi/cvent-hospitality-cloud-proposal-drafts-openapi.yml,\n  openapi/cvent-hospitality-cloud-rfp-additional-details-openapi.yml, openapi/cvent-hospitality-cloud-rfp-management-openapi.yml,\n  openapi/cvent-hospitality-cloud-rfp-requirements-openapi.yml, openapi/cvent-hospitality-cloud-rfp-suppliers-openapi.yml,\n  openapi/cvent-hospitality-cloud-signatures-openapi.yml,\
  \ openapi/cvent-hospitality-cloud-travel-accounts-openapi.yml\n  ...\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: OAuth2.clientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api-platform.cvent.com/ea/oauth2/token\n    scopes: 238\n  description: OAuth2 Client Credentials Flow.\n  sources:\n  - openapi/cvent-hospitality-cloud-authentication-openapi.yml\n  - openapi/cvent-hospitality-cloud-event-travel-openapi.yml\n  - openapi/cvent-hospitality-cloud-housing-hotels-openapi.yml\n  - openapi/cvent-hospitality-cloud-housing-openapi.yml\n  - openapi/cvent-hospitality-cloud-meeting-requests-openapi.yml\n  - openapi/cvent-hospitality-cloud-proposal-drafts-openapi.yml\n  - openapi/cvent-hospitality-cloud-rfp-additional-details-openapi.yml\n  - openapi/cvent-hospitality-cloud-rfp-management-openapi.yml\n  - openapi/cvent-hospitality-cloud-rfp-requirements-openapi.yml\n  - openapi/cvent-hospitality-cloud-rfp-suppliers-openapi.yml\n\
  \  - openapi/cvent-hospitality-cloud-signatures-openapi.yml\n  - openapi/cvent-hospitality-cloud-travel-accounts-openapi.yml\n  - openapi/cvent-hospitality-cloud-travel-rfps-openapi.yml\n  - openapi/cvent-hospitality-cloud-travel-suppliers-openapi.yml\n  - openapi/cvent-hospitality-cloud-venue-meeting-rooms-openapi.yml\n  - openapi/cvent-hospitality-cloud-venue-profiles-openapi.yml\n- name: OAuth2.authorizationCode\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api-platform.cvent.com/ea/oauth2/authorize\n    tokenUrl: https://api-platform.cvent.com/ea/oauth2/token\n    scopes: 208\n  description: OAuth2 Authorization Code Flow.\n  sources:\n  - openapi/cvent-hospitality-cloud-authentication-openapi.yml\n  - openapi/cvent-hospitality-cloud-event-travel-openapi.yml\n  - openapi/cvent-hospitality-cloud-meeting-requests-openapi.yml\n  - openapi/cvent-hospitality-cloud-rfp-additional-details-openapi.yml\n  - openapi/cvent-hospitality-cloud-rfp-management-openapi.yml\n\
  \  - openapi/cvent-hospitality-cloud-rfp-requirements-openapi.yml\n  - openapi/cvent-hospitality-cloud-rfp-suppliers-openapi.yml\n  - openapi/cvent-hospitality-cloud-signatures-openapi.yml\n  - openapi/cvent-hospitality-cloud-travel-rfps-openapi.yml\n  - openapi/cvent-hospitality-cloud-venue-meeting-rooms-openapi.yml\n  - openapi/cvent-hospitality-cloud-venue-profiles-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cvent-hospitality-cloud/refs/heads/main/authentication/cvent-hospitality-cloud-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Catering
- Group Bookings
- Hospitality
- Hospitality Cloud
- Hotels
- Housing
- Authentication
- Passkey
- Reservations
- RFP
- Room Blocks
- Sales
- Sourcing
- Supplier Network
- Venues
---
