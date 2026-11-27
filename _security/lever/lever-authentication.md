---
anonymous_access: false
api_key_in: []
api_specs:
- filename: lever-candidates-api-openapi.yml
  format: yaml
  label: Lever Candidates API
  slug: lever-candidates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lever/openapi/lever-candidates-api-openapi.yml
- filename: lever-feedback-templates-api-openapi.yml
  format: yaml
  label: Lever Feedback Templates API
  slug: lever-feedback-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lever/openapi/lever-feedback-templates-api-openapi.yml
- filename: lever-webhooks-api-openapi.yml
  format: yaml
  label: Lever Webhooks API
  slug: lever-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lever/openapi/lever-webhooks-api-openapi.yml
- filename: lever-applications-api-openapi.yml
  format: yaml
  label: Lever Applications API
  slug: lever-applications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lever/openapi/lever-applications-api-openapi.yml
- filename: lever-contacts-api-openapi.yml
  format: yaml
  label: Lever Contacts API
  slug: lever-contacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lever/openapi/lever-contacts-api-openapi.yml
- filename: lever-eeo-api-openapi.yml
  format: yaml
  label: Lever EEO API
  slug: lever-eeo-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lever/openapi/lever-eeo-api-openapi.yml
- filename: lever-files-api-openapi.yml
  format: yaml
  label: Lever Files API
  slug: lever-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lever/openapi/lever-files-api-openapi.yml
- filename: lever-opportunities-api-openapi.yml
  format: yaml
  label: Lever Opportunities API
  slug: lever-opportunities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lever/openapi/lever-opportunities-api-openapi.yml
- filename: lever-postings-api-openapi.yml
  format: yaml
  label: Lever Postings API
  slug: lever-postings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lever/openapi/lever-postings-api-openapi.yml
- filename: lever-requisitions-api-openapi.yml
  format: yaml
  label: Lever Requisitions API
  slug: lever-requisitions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lever/openapi/lever-requisitions-api-openapi.yml
- filename: lever-sources-api-openapi.yml
  format: yaml
  label: Lever Sources API
  slug: lever-sources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lever/openapi/lever-sources-api-openapi.yml
- filename: lever-stages-api-openapi.yml
  format: yaml
  label: Lever Stages API
  slug: lever-stages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lever/openapi/lever-stages-api-openapi.yml
- filename: lever-tags-api-openapi.yml
  format: yaml
  label: Lever Tags API
  slug: lever-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lever/openapi/lever-tags-api-openapi.yml
- filename: lever-users-api-openapi.yml
  format: yaml
  label: Lever Users API
  slug: lever-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lever/openapi/lever-users-api-openapi.yml
- filename: lever-archive-reasons-api-openapi.yml
  format: yaml
  label: Lever Archive Reasons API
  slug: lever-archive-reasons-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lever/openapi/lever-archive-reasons-api-openapi.yml
- filename: lever-audit-events-api-openapi.yml
  format: yaml
  label: Lever Audit Events API
  slug: lever-audit-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lever/openapi/lever-audit-events-api-openapi.yml
- filename: lever-candidates-api-openapi.yml
  format: yaml
  label: Lever Candidates API
  slug: lever-candidates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lever/openapi/lever-candidates-api-openapi.yml
- filename: lever-disposition-stages-api-openapi.yml
  format: yaml
  label: Lever Disposition Stages API
  slug: lever-disposition-stages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lever/openapi/lever-disposition-stages-api-openapi.yml
- filename: lever-feedback-templates-api-openapi.yml
  format: yaml
  label: Lever Feedback Templates API
  slug: lever-feedback-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lever/openapi/lever-feedback-templates-api-openapi.yml
- filename: lever-form-templates-api-openapi.yml
  format: yaml
  label: Lever Form Templates API
  slug: lever-form-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lever/openapi/lever-form-templates-api-openapi.yml
- filename: lever-profile-forms-api-openapi.yml
  format: yaml
  label: Lever Profile Forms API
  slug: lever-profile-forms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lever/openapi/lever-profile-forms-api-openapi.yml
- filename: lever-requisition-fields-api-openapi.yml
  format: yaml
  label: Lever Requisition Fields API
  slug: lever-requisition-fields-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lever/openapi/lever-requisition-fields-api-openapi.yml
- filename: lever-surveys-api-openapi.yml
  format: yaml
  label: Lever Surveys API
  slug: lever-surveys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lever/openapi/lever-surveys-api-openapi.yml
- filename: lever-webhooks-api-openapi.yml
  format: yaml
  label: Lever Webhooks API
  slug: lever-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lever/openapi/lever-webhooks-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Lever Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lever secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Lever
provider_slug: lever
scheme_count: 3
schemes:
- description: API key supplied as the basic auth username with empty password.
  detail: Authenticate to the Lever API via basic auth by providing an API key as the username and leaving the password blank. Create and manage your API keys from the Integrations and API page in Settings of your Lever account, on the API Credentials tab. Access to confidential data may only be granted during key creation.
  docs: https://hire.lever.co/developer/documentation#authentication
  name: basicAuth
  scheme: basic
  sources:
  - openapi/lever-applications-api-openapi.yml
  - openapi/lever-archive-reasons-api-openapi.yml
  - openapi/lever-audit-events-api-openapi.yml
  - '... (all 19 refined per-resource contracts)'
  type: http
- description: OAuth 2.0 bearer access token (Lever Partner OAuth apps).
  detail: The type of token returned is Bearer. This value must be specified along with the access token when making authenticated requests. Tokens are issued by the Lever OAuth 2.0 server (see the oauth2 scheme).
  docs: https://hire.lever.co/developer/documentation#authentication
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/lever-applications-api-openapi.yml
  - openapi/lever-archive-reasons-api-openapi.yml
  - openapi/lever-audit-events-api-openapi.yml
  - '... (all 19 refined per-resource contracts)'
  type: http
- description: OAuth is part of our partner integration program, and apps must be registered. As of 2020, all Lever integrations are authenticated using OAuth.
  discovery:
    note: 'Fetched 2026-11-05 (HTTP 200): issuer https://auth.lever.co/, S256 PKCE, client_secret_basic/post and private_key_jwt token auth, revocation at https://auth.lever.co/oauth/revoke. The Lever resource scopes are not in scopes_supported (Auth0 tenant lists OIDC scopes only).'
    oauth_authorization_server: https://auth.lever.co/.well-known/oauth-authorization-server
    openid_configuration: https://auth.lever.co/.well-known/openid-configuration
    saved:
    - well-known/lever-auth-oauth-authorization-server.json
    - well-known/lever-auth-openid-configuration.json
  docs: https://hire.lever.co/developer/oauth
  flows:
    authorizationCode:
      authorizationUrl: https://auth.lever.co/authorize
      refreshUrl: https://auth.lever.co/oauth/token
      scopes:
        applications:read:admin: View all opportunity applications
        archive_reasons:read:admin: View all archived reasons
        audit_events:read:admin: View all audit events
        contact:read:admin: View an opportunity's contact
        contact:write:admin: View and manage an opportunity's contact
        diversity_surveys:read:admin: View all diversity surveys
        eeo_responses:read:admin: View all EEO responses without personally identifiable information
        eeo_responses_pii:read:admin: View all EEO responses with or without personally identifiable information
        feedback:read:admin: View all of an opportunity's feedback
        feedback:write:admin: View and manage all of an opportunity's feedback
        feedback_templates:read:admin: View all feedback templates
        feedback_templates:write:admin: View and manage all feedback templates
        files:read:admin: View all of an opportunity's files
        files:write:admin: View and manage all of an opportunity's files
        form_templates:read:admin: View all form templates
        form_templates:write:admin: View and manage all form templates
        forms:read:admin: View all of an opportunity's forms
        forms:write:admin: View and manage all of an opportunity's forms
        groups:read:admin: View all user groups
        groups:write:admin: View and manage all user groups
        interviews:read:admin: View all of an opportunity's interviews
        interviews:write:admin: View and manage all of an opportunity's interviews
        notes:read:admin: View all of an opportunity's notes
        notes:write:admin: View and manage all of an opportunity's notes
        offers:read:admin: View all of an opportunity's offers
        offline_access: 'Include offline_access to get a Refresh Token (Lever docs, Step 1: Request User Authorization).'
        opportunities:read:admin: required
        opportunities:write:admin: View and manage all opportunities
        panels:read:admin: View all of an opportunity's panels
        panels:write:admin: View and manage all of an opportunity's panels
        permissions:read:admin: View all user or role permissions
        permissions:write:admin: View and manage all user or role permissions
        postings:read:admin: View all postings
        postings:write:admin: View and manage all postings
        referrals:read:admin: View all of an opportunity's referrals
        requisition_fields:read:admin: View all requisition fields
        requisition_fields:write:admin: View and manage all requisition fields
        requisitions:read:admin: View all requisitions
        requisitions:write:admin: View and manage all requisitions
        resumes:read:admin: View all of an opportunity's resumes
        roles:read:admin: View all roles
        roles:write:admin: View and manage all roles
        sources:read:admin: View all sources
        stages:read:admin: View all stages
        tags:read:admin: View all tags
        tasks:read:admin: View all tasks
        uploads:write:admin: Manage all file uploads
        users:read:admin: View all users
        users:write:admin: View and manage all users
        webhooks:read:admin: View all webhooks
        webhooks:write:admin: Manage all webhooks
      tokenUrl: https://auth.lever.co/oauth/token
  name: leverOAuth
  refresh_tokens: Include offline_access to get a Refresh Token; access tokens expire and are refreshed without the customer re-authenticating.
  registration: Partner apps are registered with Lever (integration name, 20-140 character description, callback URL(s), square logo, required scopes; maximum 20 scopes). Separate apps exist for sandbox and production.
  required_authorize_params:
  - client_id
  - redirect_uri
  - response_type=code
  - state
  - audience=https://api.lever.co/v1/
  - scope
  sandbox:
    audience: https://api.sandbox.lever.co/v1/
    authorizationUrl: https://sandbox-lever.auth0.com/authorize
  sources:
  - https://hire.lever.co/developer/oauth
  - https://hire.lever.co/developer/documentation#authentication
  type: oauth2
slug: lever-authentication
source_filename: lever-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: searched\nsource: https://hire.lever.co/developer/documentation#authentication\nsummary:\n  types:\n  - http\n  - oauth2\n  customer_path: API key (basic auth) created by a Super Admin in Settings; endpoint access and confidential-data\n    access chosen at key creation\n  partner_path: OAuth 2.0 authorization code with refresh tokens; Super Admins authorize an app once for the whole\n    organization and can revoke it from settings\n  eu: OAuth is supported for customers in the EU. Any integration authorization or action will be re-directed automatically\n    to the appropriate data center.\n  derived_from: derive-authentication.py over the 19 refined per-resource contracts (basicAuth, bearerAuth), upgraded\n    from the documentation on 2026-11-05\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: API key supplied as the basic auth username with empty password.\n  sources:\n  - openapi/lever-applications-api-openapi.yml\n\
  \  - openapi/lever-archive-reasons-api-openapi.yml\n  - openapi/lever-audit-events-api-openapi.yml\n  - '... (all 19 refined per-resource contracts)'\n  docs: https://hire.lever.co/developer/documentation#authentication\n  detail: Authenticate to the Lever API via basic auth by providing an API key as the username and leaving the password\n    blank. Create and manage your API keys from the Integrations and API page in Settings of your Lever account,\n    on the API Credentials tab. Access to confidential data may only be granted during key creation.\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth 2.0 bearer access token (Lever Partner OAuth apps).\n  sources:\n  - openapi/lever-applications-api-openapi.yml\n  - openapi/lever-archive-reasons-api-openapi.yml\n  - openapi/lever-audit-events-api-openapi.yml\n  - '... (all 19 refined per-resource contracts)'\n  docs: https://hire.lever.co/developer/documentation#authentication\n  detail: The type of token returned\
  \ is Bearer. This value must be specified along with the access token when making\n    authenticated requests. Tokens are issued by the Lever OAuth 2.0 server (see the oauth2 scheme).\n- name: leverOAuth\n  type: oauth2\n  description: OAuth is part of our partner integration program, and apps must be registered. As of 2020, all Lever\n    integrations are authenticated using OAuth.\n  docs: https://hire.lever.co/developer/oauth\n  flows:\n    authorizationCode:\n      authorizationUrl: https://auth.lever.co/authorize\n      tokenUrl: https://auth.lever.co/oauth/token\n      refreshUrl: https://auth.lever.co/oauth/token\n      scopes:\n        applications:read:admin: View all opportunity applications\n        archive_reasons:read:admin: View all archived reasons\n        audit_events:read:admin: View all audit events\n        contact:read:admin: View an opportunity's contact\n        contact:write:admin: View and manage an opportunity's contact\n        diversity_surveys:read:admin: View\
  \ all diversity surveys\n        eeo_responses:read:admin: View all EEO responses without personally identifiable information\n        eeo_responses_pii:read:admin: View all EEO responses with or without personally identifiable information\n        feedback:read:admin: View all of an opportunity's feedback\n        feedback:write:admin: View and manage all of an opportunity's feedback\n        feedback_templates:read:admin: View all feedback templates\n        feedback_templates:write:admin: View and manage all feedback templates\n        files:read:admin: View all of an opportunity's files\n        files:write:admin: View and manage all of an opportunity's files\n        form_templates:read:admin: View all form templates\n        form_templates:write:admin: View and manage all form templates\n        forms:read:admin: View all of an opportunity's forms\n        forms:write:admin: View and manage all of an opportunity's forms\n        groups:read:admin: View all user groups\n        groups:write:admin:\
  \ View and manage all user groups\n        interviews:read:admin: View all of an opportunity's interviews\n        interviews:write:admin: View and manage all of an opportunity's interviews\n        notes:read:admin: View all of an opportunity's notes\n        notes:write:admin: View and manage all of an opportunity's notes\n        offers:read:admin: View all of an opportunity's offers\n        opportunities:read:admin: required\n        opportunities:write:admin: View and manage all opportunities\n        panels:read:admin: View all of an opportunity's panels\n        panels:write:admin: View and manage all of an opportunity's panels\n        permissions:read:admin: View all user or role permissions\n        permissions:write:admin: View and manage all user or role permissions\n        postings:read:admin: View all postings\n        postings:write:admin: View and manage all postings\n        referrals:read:admin: View all of an opportunity's referrals\n        requisition_fields:read:admin:\
  \ View all requisition fields\n        requisition_fields:write:admin: View and manage all requisition fields\n        requisitions:read:admin: View all requisitions\n        requisitions:write:admin: View and manage all requisitions\n        resumes:read:admin: View all of an opportunity's resumes\n        roles:read:admin: View all roles\n        roles:write:admin: View and manage all roles\n        sources:read:admin: View all sources\n        stages:read:admin: View all stages\n        tags:read:admin: View all tags\n        tasks:read:admin: View all tasks\n        uploads:write:admin: Manage all file uploads\n        users:read:admin: View all users\n        users:write:admin: View and manage all users\n        webhooks:read:admin: View all webhooks\n        webhooks:write:admin: Manage all webhooks\n        offline_access: 'Include offline_access to get a Refresh Token (Lever docs, Step 1: Request User Authorization).'\n  required_authorize_params:\n  - client_id\n  - redirect_uri\n\
  \  - response_type=code\n  - state\n  - audience=https://api.lever.co/v1/\n  - scope\n  refresh_tokens: Include offline_access to get a Refresh Token; access tokens expire and are refreshed without\n    the customer re-authenticating.\n  sandbox:\n    authorizationUrl: https://sandbox-lever.auth0.com/authorize\n    audience: https://api.sandbox.lever.co/v1/\n  discovery:\n    oauth_authorization_server: https://auth.lever.co/.well-known/oauth-authorization-server\n    openid_configuration: https://auth.lever.co/.well-known/openid-configuration\n    saved:\n    - well-known/lever-auth-oauth-authorization-server.json\n    - well-known/lever-auth-openid-configuration.json\n    note: 'Fetched 2026-11-05 (HTTP 200): issuer https://auth.lever.co/, S256 PKCE, client_secret_basic/post and\n      private_key_jwt token auth, revocation at https://auth.lever.co/oauth/revoke. The Lever resource scopes are\n      not in scopes_supported (Auth0 tenant lists OIDC scopes only).'\n  registration: Partner\
  \ apps are registered with Lever (integration name, 20-140 character description, callback\n    URL(s), square logo, required scopes; maximum 20 scopes). Separate apps exist for sandbox and production.\n  sources:\n  - https://hire.lever.co/developer/oauth\n  - https://hire.lever.co/developer/documentation#authentication\ndocs: https://hire.lever.co/developer/documentation#authentication\nscopes_artifact: scopes/lever-scopes.yml\ndocs_also: https://hire.lever.co/developer/oauth\n"
source_yaml_url: https://artifacts.apis.io/lever/authentication/lever-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Human Resources
- Applicant Tracking
- Recruiting
- Talent Acquisition
- Software-as-a-Service
---
