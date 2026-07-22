---
api_key_in: []
auth_types:
- openIdConnect
description: ''
kind: authentication
layout: security
method: probed
name: Lane Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lane secures its APIs with openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Lane
provider_slug: lane
scheme_count: 2
schemes:
- applies_to: VTS Activate web and mobile application sign-in
  evidence: The application shell embeds an x-whitelabel meta payload containing "auth0OrganizationId":"org_TkmIkPNpHVBXGFMX" and "isMagicLinkEnabled":false, alongside "settings":{"allowSignUps":true,"emailSubscriptionOptIn":true}.
  name: Auth0 tenant SSO
  organization_id: org_TkmIkPNpHVBXGFMX
  provider: Auth0
  source: https://app.joinlane.com/
  type: openIdConnect
- applies_to: VTS platform sign-in
  evidence: The VTS status page tracks an "SSO/Login" component covering platform authentication.
  name: Platform SSO/Login
  source: https://status.vts.com/
  type: unknown
slug: lane-authentication
source_filename: lane-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: >-\n  Embedded whitelabel configuration and JavaScript bundle served by https://app.joinlane.com/ and\n  https://assets.activate.vts.com/static/\napi_auth_documented: false\nnote: >-\n  Lane publishes no OpenAPI definition, no developer portal and no authentication documentation, so\n  there is nothing to derive a securityScheme profile from and no Authentication pointer is wired in\n  apis.yml. What is recorded below is the observable end-user identity mechanism of the VTS Activate\n  application itself, captured so a later round does not have to rediscover it. It is an application\n  sign-in profile, not a documented API authentication contract.\nsummary:\n  types:\n  - openIdConnect\n  identity_provider: Auth0\n  end_user_signup_allowed: true\n  magic_link_enabled: false\nschemes:\n- name: Auth0 tenant SSO\n  type: openIdConnect\n  provider: Auth0\n  organization_id: org_TkmIkPNpHVBXGFMX\n  applies_to: VTS Activate web and\
  \ mobile application sign-in\n  source: https://app.joinlane.com/\n  evidence: >-\n    The application shell embeds an x-whitelabel meta payload containing\n    \"auth0OrganizationId\":\"org_TkmIkPNpHVBXGFMX\" and \"isMagicLinkEnabled\":false, alongside\n    \"settings\":{\"allowSignUps\":true,\"emailSubscriptionOptIn\":true}.\n- name: Platform SSO/Login\n  type: unknown\n  applies_to: VTS platform sign-in\n  source: https://status.vts.com/\n  evidence: The VTS status page tracks an \"SSO/Login\" component covering platform authentication.\napi_surface:\n  style: graphql\n  public: false\n  documented: false\n  evidence: >-\n    The application bundle at\n    https://assets.activate.vts.com/static/main.64f2999eb29bba37a547.js uses an Apollo GraphQL client\n    with operations including user.forgotPassword, user.requestAccountDeletion, user.updateUser,\n    getUserLogins, getProxyClickCompanies and queryChannelInvitesByGroupRole. No GraphQL endpoint,\n    schema or introspection surface\
  \ is publicly documented, and no attempt was made to query it.\n  note: >-\n    The VTS status page lists an \"APIs\" component, indicating the parent platform operates APIs, but\n    no developer documentation for them is published (developer.vts.com and docs.vts.com do not\n    resolve; api.vts.com serves no OpenAPI, Swagger or docs path).\nthird_party_integrations_observed:\n- {name: Stripe, purpose: in-app retail and food-service payments, evidence: https://js.stripe.com/v3/ loaded by the app shell}\n- {name: Google Maps, purpose: mapping, evidence: https://maps.googleapis.com/maps/api/js loaded by the app shell}\n- {name: Pendo, purpose: product analytics and in-app guides, evidence: content.p.activate.vts.com resolves to pendo.io}\n- {name: Retool, purpose: embedded internal tooling, evidence: retool.vts.com embedded public app referenced in the bundle}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lane/refs/heads/main/authentication/lane-authentication.yml
summary_line: openIdConnect · 2 schemes
tags:
- Company
- Real Estate
- Commercial Real Estate
- Property Technology
- Workplace
- Tenant Experience
- Building Access
- Visitor Management
- Amenity Booking
- Mobile
---
