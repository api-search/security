---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Linkable Networks Collinson Group Authentication
name_suffix: Authentication
oauth_flows: []
overview: Linkable Networks (Collinson Group) declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Linkable Networks (Collinson Group)
provider_slug: linkable-networks-collinson-group
scheme_count: 1
schemes:
- documented: true
  evidence: '"Authentication Method: OAuth 2.0 (Specifically the API supports OAuth''s Resource Owner Password Credentials as described in section 4.3.)"'
  flow: password
  id: oauth2_password
  scopes: []
  scopes_note: No scope reference is published. Authorization appears to be partner-tier based rather than scope-based - adding and updating payment cards is limited to PCI-compliant partners.
  spec: RFC 6749 section 4.3 (Resource Owner Password Credentials Grant)
  token_url: null
  token_url_note: Not published on any public Linkable Networks or MyLinkables surface.
  type: oauth2
slug: linkable-networks-collinson-group-authentication
source_filename: linkable-networks-collinson-group-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://linkablenetworks.com/appweb-developers/\ndocs: https://linkablenetworks.com/appweb-developers/\napi: MyLinkables Consumer API\nbase_url: https://api.mylinkables.com\nsummary: >-\n  The MyLinkables Consumer API authenticates with OAuth 2.0, specifically the Resource Owner Password\n  Credentials grant described in RFC 6749 section 4.3. The provider states \"if you know REST and OAuth you\n  know our API\". Credentials are not self-service: partners request API documentation and credentials by\n  email from Linkable Networks. No token, authorize or introspection endpoint is published publicly, and\n  the host serves no OAuth or OpenID discovery document.\nschemes:\n- id: oauth2_password\n  type: oauth2\n  flow: password\n  spec: RFC 6749 section 4.3 (Resource Owner Password Credentials Grant)\n  documented: true\n  evidence: >-\n    \"Authentication Method: OAuth 2.0 (Specifically the API supports OAuth's Resource Owner\
  \ Password\n    Credentials as described in section 4.3.)\"\n  token_url: null\n  token_url_note: Not published on any public Linkable Networks or MyLinkables surface.\n  scopes: []\n  scopes_note: >-\n    No scope reference is published. Authorization appears to be partner-tier based rather than\n    scope-based - adding and updating payment cards is limited to PCI-compliant partners.\ncredential_issuance:\n  self_service: false\n  method: email request\n  evidence: >-\n    \"Send us an email with your contact information and we'll send along our API documentation and your\n    credentials.\"\n  contact_page: https://linkablenetworks.com/contact/\ndiscovery:\n  openid_configuration: 404\n  oauth_authorization_server: 404\n  note: Probed 2026-07-19 against https://api.mylinkables.com - neither discovery document is served.\nobserved:\n  probed: '2026-07-19'\n  note: >-\n    Unauthenticated GET against the documented consumerapi paths returns HTTP 403 with a page titled\n    \"consumerapi.accessdenied.title\"\
  , confirming the endpoints exist and are auth-gated. Undocumented\n    paths on the same host return 404.\n  response_headers:\n    strict_transport_security: max-age=31536000; includeSubDomains; preload\n    x_content_type_options: nosniff\n    x_frame_options: SAMEORIGIN\n    access_control_allow_origin: '*'\n    access_control_allow_credentials: 'true'\ngaps:\n- No public token endpoint or OAuth discovery document.\n- No published scope or permission reference.\n- Resource Owner Password Credentials is deprecated by OAuth 2.0 Security Best Current Practice (RFC 9700)\n  and removed from OAuth 2.1; no alternative grant (authorization code + PKCE, client credentials) is\n  documented.\n- Documentation is gated behind an email request, so the authentication contract cannot be fully verified.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/linkable-networks-collinson-group/refs/heads/main/authentication/linkable-networks-collinson-group-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Fintech
- Card Linked Offers
- Loyalty
- Payments
- Rewards
- Advertising
- Retail
---
