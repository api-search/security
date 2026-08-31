---
api_key_in:
- header
api_specs:
- filename: constant-contact-account-services-api-openapi.yml
  format: yaml
  label: Constant Contact Account Services API
  slug: constant-contact-account-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constant-contact/refs/heads/main/openapi/constant-contact-account-services-api-openapi.yml
- filename: constant-contact-bulk-activities-api-openapi.yml
  format: yaml
  label: Constant Contact Bulk Activities API
  slug: constant-contact-bulk-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constant-contact/refs/heads/main/openapi/constant-contact-bulk-activities-api-openapi.yml
- filename: constant-contact-contact-lists-api-openapi.yml
  format: yaml
  label: Constant Contact Contact Lists API
  slug: constant-contact-contact-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constant-contact/refs/heads/main/openapi/constant-contact-contact-lists-api-openapi.yml
- filename: constant-contact-contact-tags-api-openapi.yml
  format: yaml
  label: Constant Contact Contact Tags API
  slug: constant-contact-contact-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constant-contact/refs/heads/main/openapi/constant-contact-contact-tags-api-openapi.yml
- filename: constant-contact-contacts-api-openapi.yml
  format: yaml
  label: Constant Contact Contacts API
  slug: constant-contact-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constant-contact/refs/heads/main/openapi/constant-contact-contacts-api-openapi.yml
- filename: constant-contact-contacts-custom-fields-api-openapi.yml
  format: yaml
  label: Constant Contact Contacts Custom Fields API
  slug: constant-contact-contacts-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constant-contact/refs/heads/main/openapi/constant-contact-contacts-custom-fields-api-openapi.yml
- filename: constant-contact-contacts-reporting-api-openapi.yml
  format: yaml
  label: Constant Contact Contacts Reporting API
  slug: constant-contact-contacts-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constant-contact/refs/heads/main/openapi/constant-contact-contacts-reporting-api-openapi.yml
- filename: constant-contact-email-campaigns-ab-tests-api-openapi.yml
  format: yaml
  label: Constant Contact Email Campaigns AB Tests API
  slug: constant-contact-email-campaigns-ab-tests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constant-contact/refs/heads/main/openapi/constant-contact-email-campaigns-ab-tests-api-openapi.yml
- filename: constant-contact-email-campaigns-api-openapi.yml
  format: yaml
  label: Constant Contact Email Campaigns API
  slug: constant-contact-email-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constant-contact/refs/heads/main/openapi/constant-contact-email-campaigns-api-openapi.yml
- filename: constant-contact-email-reporting-api-openapi.yml
  format: yaml
  label: Constant Contact Email Reporting API
  slug: constant-contact-email-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constant-contact/refs/heads/main/openapi/constant-contact-email-reporting-api-openapi.yml
- filename: constant-contact-email-scheduling-api-openapi.yml
  format: yaml
  label: Constant Contact Email Scheduling API
  slug: constant-contact-email-scheduling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constant-contact/refs/heads/main/openapi/constant-contact-email-scheduling-api-openapi.yml
- filename: constant-contact-events-api-openapi.yml
  format: yaml
  label: Constant Contact Events API
  slug: constant-contact-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constant-contact/refs/heads/main/openapi/constant-contact-events-api-openapi.yml
- filename: constant-contact-landing-pages-reporting-api-openapi.yml
  format: yaml
  label: Constant Contact Landing Pages Reporting API
  slug: constant-contact-landing-pages-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constant-contact/refs/heads/main/openapi/constant-contact-landing-pages-reporting-api-openapi.yml
- filename: constant-contact-segments-api-openapi.yml
  format: yaml
  label: Constant Contact Segments API
  slug: constant-contact-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constant-contact/refs/heads/main/openapi/constant-contact-segments-api-openapi.yml
- filename: constant-contact-sms-reporting-api-openapi.yml
  format: yaml
  label: Constant Contact SMS Reporting API
  slug: constant-contact-sms-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constant-contact/refs/heads/main/openapi/constant-contact-sms-reporting-api-openapi.yml
- filename: constant-contact-technology-partners-api-openapi.yml
  format: yaml
  label: Constant Contact Technology Partners API
  slug: constant-contact-technology-partners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constant-contact/refs/heads/main/openapi/constant-contact-technology-partners-api-openapi.yml
- filename: constant-contact-technology-partners-webhooks-api-openapi.yml
  format: yaml
  label: Constant Contact Technology Partners Webhooks API
  slug: constant-contact-technology-partners-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constant-contact/refs/heads/main/openapi/constant-contact-technology-partners-webhooks-api-openapi.yml
- filename: constant-contact-automations-api-openapi.yml
  format: yaml
  label: Constant Contact Automations API
  slug: constant-contact-automations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constant-contact/refs/heads/main/openapi/constant-contact-automations-api-openapi.yml
- filename: constant-contact-social-api-openapi.yml
  format: yaml
  label: Constant Contact Social API
  slug: constant-contact-social-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constant-contact/refs/heads/main/openapi/constant-contact-social-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: 'Constant Contact V3 authenticates every request with an OAuth2 JWT bearer access token. There is no API-key-only path to the API: the value the developer portal calls an "API key" IS the OAuth2 client_id, not a standalone credential.'
kind: authentication
layout: security
method: searched
name: Constant Contact Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
overview: Constant Contact secures its APIs with apiKey and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and implicit flow(s).
provider_name: Constant Contact
provider_slug: constant-contact
scheme_count: 3
schemes:
- flows:
  - authorizationUrl: https://authz.constantcontact.com/oauth2/default/v1/authorize
    flow: implicit
    scopes: 4
  name: oauth2_implicit
  sources:
  - openapi/constant-contact-account-services-api-openapi.yml
  - openapi/constant-contact-bulk-activities-api-openapi.yml
  - openapi/constant-contact-contact-lists-api-openapi.yml
  - openapi/constant-contact-contact-tags-api-openapi.yml
  - openapi/constant-contact-contacts-api-openapi.yml
  - openapi/constant-contact-contacts-custom-fields-api-openapi.yml
  - openapi/constant-contact-contacts-reporting-api-openapi.yml
  - openapi/constant-contact-email-campaigns-ab-tests-api-openapi.yml
  - openapi/constant-contact-email-campaigns-api-openapi.yml
  - openapi/constant-contact-email-reporting-api-openapi.yml
  - openapi/constant-contact-email-scheduling-api-openapi.yml
  - openapi/constant-contact-events-api-openapi.yml
  - openapi/constant-contact-landing-pages-reporting-api-openapi.yml
  - openapi/constant-contact-segments-api-openapi.yml
  - openapi/constant-contact-sms-reporting-api-openapi.yml
  - openapi/constant-contact-technology-partners-api-openapi.yml
  - openapi/constant-contact-technology-partners-webhooks-api-openapi.yml
  type: oauth2
- flows:
  - authorizationUrl: https://authz.constantcontact.com/oauth2/default/v1/authorize
    flow: authorizationCode
    scopes: 4
    tokenUrl: https://authz.constantcontact.com/oauth2/default/v1/token
  name: oauth2_access_code
  sources:
  - openapi/constant-contact-account-services-api-openapi.yml
  - openapi/constant-contact-bulk-activities-api-openapi.yml
  - openapi/constant-contact-contact-lists-api-openapi.yml
  - openapi/constant-contact-contact-tags-api-openapi.yml
  - openapi/constant-contact-contacts-api-openapi.yml
  - openapi/constant-contact-contacts-custom-fields-api-openapi.yml
  - openapi/constant-contact-contacts-reporting-api-openapi.yml
  - openapi/constant-contact-email-campaigns-ab-tests-api-openapi.yml
  - openapi/constant-contact-email-campaigns-api-openapi.yml
  - openapi/constant-contact-email-reporting-api-openapi.yml
  - openapi/constant-contact-email-scheduling-api-openapi.yml
  - openapi/constant-contact-events-api-openapi.yml
  - openapi/constant-contact-landing-pages-reporting-api-openapi.yml
  - openapi/constant-contact-segments-api-openapi.yml
  - openapi/constant-contact-sms-reporting-api-openapi.yml
  - openapi/constant-contact-technology-partners-api-openapi.yml
  - openapi/constant-contact-technology-partners-webhooks-api-openapi.yml
  type: oauth2
- in: header
  name: api_key
  parameter: x-api-key
  sources:
  - openapi/constant-contact-account-services-api-openapi.yml
  - openapi/constant-contact-bulk-activities-api-openapi.yml
  - openapi/constant-contact-contact-lists-api-openapi.yml
  - openapi/constant-contact-contact-tags-api-openapi.yml
  - openapi/constant-contact-contacts-api-openapi.yml
  - openapi/constant-contact-contacts-custom-fields-api-openapi.yml
  - openapi/constant-contact-contacts-reporting-api-openapi.yml
  - openapi/constant-contact-email-campaigns-ab-tests-api-openapi.yml
  - openapi/constant-contact-email-campaigns-api-openapi.yml
  - openapi/constant-contact-email-reporting-api-openapi.yml
  - openapi/constant-contact-email-scheduling-api-openapi.yml
  - openapi/constant-contact-events-api-openapi.yml
  - openapi/constant-contact-landing-pages-reporting-api-openapi.yml
  - openapi/constant-contact-segments-api-openapi.yml
  - openapi/constant-contact-sms-reporting-api-openapi.yml
  - openapi/constant-contact-technology-partners-api-openapi.yml
  - openapi/constant-contact-technology-partners-webhooks-api-openapi.yml
  type: apiKey
slug: constant-contact-authentication
source_filename: constant-contact-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://developer.constantcontact.com/api_guide/auth_overview.html + https://developer.constantcontact.com/api_guide/scopes.html\n  + openapi/_original/constant-contact-v3-openapi.yml (build 3.0.178)\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  - implicit\nschemes:\n- name: oauth2_implicit\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://authz.constantcontact.com/oauth2/default/v1/authorize\n    scopes: 4\n  sources:\n  - openapi/constant-contact-account-services-api-openapi.yml\n  - openapi/constant-contact-bulk-activities-api-openapi.yml\n  - openapi/constant-contact-contact-lists-api-openapi.yml\n  - openapi/constant-contact-contact-tags-api-openapi.yml\n  - openapi/constant-contact-contacts-api-openapi.yml\n  - openapi/constant-contact-contacts-custom-fields-api-openapi.yml\n  - openapi/constant-contact-contacts-reporting-api-openapi.yml\n\
  \  - openapi/constant-contact-email-campaigns-ab-tests-api-openapi.yml\n  - openapi/constant-contact-email-campaigns-api-openapi.yml\n  - openapi/constant-contact-email-reporting-api-openapi.yml\n  - openapi/constant-contact-email-scheduling-api-openapi.yml\n  - openapi/constant-contact-events-api-openapi.yml\n  - openapi/constant-contact-landing-pages-reporting-api-openapi.yml\n  - openapi/constant-contact-segments-api-openapi.yml\n  - openapi/constant-contact-sms-reporting-api-openapi.yml\n  - openapi/constant-contact-technology-partners-api-openapi.yml\n  - openapi/constant-contact-technology-partners-webhooks-api-openapi.yml\n- name: oauth2_access_code\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://authz.constantcontact.com/oauth2/default/v1/authorize\n    tokenUrl: https://authz.constantcontact.com/oauth2/default/v1/token\n    scopes: 4\n  sources:\n  - openapi/constant-contact-account-services-api-openapi.yml\n  - openapi/constant-contact-bulk-activities-api-openapi.yml\n\
  \  - openapi/constant-contact-contact-lists-api-openapi.yml\n  - openapi/constant-contact-contact-tags-api-openapi.yml\n  - openapi/constant-contact-contacts-api-openapi.yml\n  - openapi/constant-contact-contacts-custom-fields-api-openapi.yml\n  - openapi/constant-contact-contacts-reporting-api-openapi.yml\n  - openapi/constant-contact-email-campaigns-ab-tests-api-openapi.yml\n  - openapi/constant-contact-email-campaigns-api-openapi.yml\n  - openapi/constant-contact-email-reporting-api-openapi.yml\n  - openapi/constant-contact-email-scheduling-api-openapi.yml\n  - openapi/constant-contact-events-api-openapi.yml\n  - openapi/constant-contact-landing-pages-reporting-api-openapi.yml\n  - openapi/constant-contact-segments-api-openapi.yml\n  - openapi/constant-contact-sms-reporting-api-openapi.yml\n  - openapi/constant-contact-technology-partners-api-openapi.yml\n  - openapi/constant-contact-technology-partners-webhooks-api-openapi.yml\n- name: api_key\n  type: apiKey\n  in: header\n  parameter:\
  \ x-api-key\n  sources:\n  - openapi/constant-contact-account-services-api-openapi.yml\n  - openapi/constant-contact-bulk-activities-api-openapi.yml\n  - openapi/constant-contact-contact-lists-api-openapi.yml\n  - openapi/constant-contact-contact-tags-api-openapi.yml\n  - openapi/constant-contact-contacts-api-openapi.yml\n  - openapi/constant-contact-contacts-custom-fields-api-openapi.yml\n  - openapi/constant-contact-contacts-reporting-api-openapi.yml\n  - openapi/constant-contact-email-campaigns-ab-tests-api-openapi.yml\n  - openapi/constant-contact-email-campaigns-api-openapi.yml\n  - openapi/constant-contact-email-reporting-api-openapi.yml\n  - openapi/constant-contact-email-scheduling-api-openapi.yml\n  - openapi/constant-contact-events-api-openapi.yml\n  - openapi/constant-contact-landing-pages-reporting-api-openapi.yml\n  - openapi/constant-contact-segments-api-openapi.yml\n  - openapi/constant-contact-sms-reporting-api-openapi.yml\n  - openapi/constant-contact-technology-partners-api-openapi.yml\n\
  \  - openapi/constant-contact-technology-partners-webhooks-api-openapi.yml\ndocs: https://developer.constantcontact.com/api_guide/auth_overview.html\nprovider: Constant Contact\nproviderId: constant-contact\ndescription: 'Constant Contact V3 authenticates every request with an OAuth2 JWT bearer access token.\n  There is no API-key-only path to the API: the value the developer portal calls an \"API key\" IS the OAuth2\n  client_id, not a standalone credential.'\nprofile:\n  primary: oauth2\n  header: 'Authorization: Bearer <access_token>'\n  token_format: JWT (1,000-1,200 characters)\n  authorization_url: https://authz.constantcontact.com/oauth2/default/v1/authorize\n  token_url: https://authz.constantcontact.com/oauth2/default/v1/token\n  device_authorization_url: https://authz.constantcontact.com/oauth2/default/v1/device/authorize\n  partner_token_url: https://authz.constantcontact.com/partners/oauth2/default/v1/token\n  discovery: none — /.well-known/openid-configuration and /.well-known/oauth-authorization-server\
  \ both\n    404 on authz.constantcontact.com\nflows:\n- flow: authorization_code\n  recommended_for: Traditional server-rendered web applications\n  client_secret_required: true\n  refresh_token: true\n  access_token_ttl_seconds: 86400\n  access_token_ttl_note: 1440 minutes; 24 hours is the maximum\n- flow: authorization_code_pkce\n  recommended_for: Native and single-page applications (public clients)\n  client_secret_required: false\n  refresh_token: true\n  access_token_ttl_seconds: 86400\n- flow: device\n  recommended_for: Input-constrained clients that cannot present a browser\n  client_secret_required: false\n  refresh_token: false\n  access_token_ttl_seconds: 86400\n- flow: implicit\n  recommended_for: Legacy public clients without Web Crypto support\n  client_secret_required: false\n  refresh_token: false\n  access_token_ttl_seconds: 28800\n  access_token_ttl_note: 480 minutes — shorter than the other flows\n  caution: Implicit is discouraged by OAuth 2.1 / RFC 9700. It remains\
  \ declared in the contract as securityScheme\n    oauth2_implicit.\nrefresh:\n  supported: true\n  scope_required: offline_access\n  lifetime: 180 days if never used\n  flows:\n  - authorization_code\n  - authorization_code_pkce\n  note: Not available in the implicit or device flows — those clients must re-authorize the user.\ncredentials:\n  client_id: The value the developer portal labels the \"API key\" for your integration.\n  client_secret: Required for the authorization-code flow; not used by public clients.\n  note: There is no request-signing scheme and no mTLS option.\nscopes:\n  documented:\n  - account_read\n  - account_update\n  - contact_data\n  - campaign_data\n  - offline_access\n  spec_only:\n  - v3api/general.partner\n  delimiter: space\n  see: scopes/constant-contact-scopes.yml\npartner_auth:\n  scheme: ctctPartnerAuthorizer\n  authorization_url_in_spec: https://v3api-partner.auth.us-east-1.amazoncognito.com/oauth2/token\n  documented_url: https://authz.constantcontact.com/partners/oauth2/default/v1/token\n\
  \  conflict_note: The contract still points the partner authorizer at an AWS Cognito host (v3api-partner.auth.us-east-1.amazoncognito.com)\n    while the September 2025 release notes moved partner token issuance to authz.constantcontact.com/partners/oauth2/default/v1/token.\n    The spec is stale on this point; follow the release notes.\nfindings:\n- A 403 conflates three unrelated causes — missing scope, missing user privilege, and a deactivated application\n  — so an agent cannot tell a permission problem from an account problem without calling getUserPrivileges.\n- No authorization-server metadata is published, so every endpoint must be hard-coded by the client.\n- Token TTL is long (24h) and refresh tokens live 180 days, which raises the blast radius of a leaked\n  token on an API whose contact_data scope permits bulk deletion.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/constant-contact/refs/heads/main/authentication/constant-contact-authentication.yml
summary_line: apiKey/oauth2 · 3 schemes
tags:
- Campaigns
- Contacts
- Email Marketing
- Event
- Reporting
- SMS
- Surveys
---
