---
anonymous_access: false
api_key_in: []
api_specs:
- filename: domani-run-account-api-openapi.yml
  format: yaml
  label: Domani Account API
  slug: domani-run-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domani-run/openapi/domani-run-account-api-openapi.yml
- filename: domani-run-api-tokens-api-openapi.yml
  format: yaml
  label: Domani API Tokens API
  slug: domani-run-api-tokens-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domani-run/openapi/domani-run-api-tokens-api-openapi.yml
- filename: domani-run-auth-api-openapi.yml
  format: yaml
  label: Domani Auth API
  slug: domani-run-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domani-run/openapi/domani-run-auth-api-openapi.yml
- filename: domani-run-authentication-api-openapi.yml
  format: yaml
  label: Domani Authentication API
  slug: domani-run-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domani-run/openapi/domani-run-authentication-api-openapi.yml
- filename: domani-run-backorders-api-openapi.yml
  format: yaml
  label: Domani Backorders API
  slug: domani-run-backorders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domani-run/openapi/domani-run-backorders-api-openapi.yml
- filename: domani-run-billing-api-openapi.yml
  format: yaml
  label: Domani Billing API
  slug: domani-run-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domani-run/openapi/domani-run-billing-api-openapi.yml
- filename: domani-run-collaboration-api-openapi.yml
  format: yaml
  label: Domani Collaboration API
  slug: domani-run-collaboration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domani-run/openapi/domani-run-collaboration-api-openapi.yml
- filename: domani-run-connect-api-openapi.yml
  format: yaml
  label: Domani Connect API
  slug: domani-run-connect-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domani-run/openapi/domani-run-connect-api-openapi.yml
- filename: domani-run-discovery-api-openapi.yml
  format: yaml
  label: Domani Discovery API
  slug: domani-run-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domani-run/openapi/domani-run-discovery-api-openapi.yml
- filename: domani-run-dns-api-openapi.yml
  format: yaml
  label: Domani DNS API
  slug: domani-run-dns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domani-run/openapi/domani-run-dns-api-openapi.yml
- filename: domani-run-domain-search-api-openapi.yml
  format: yaml
  label: Domani Domain Search API
  slug: domani-run-domain-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domani-run/openapi/domani-run-domain-search-api-openapi.yml
- filename: domani-run-domains-api-openapi.yml
  format: yaml
  label: Domani Domains API
  slug: domani-run-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domani-run/openapi/domani-run-domains-api-openapi.yml
- filename: domani-run-email-api-openapi.yml
  format: yaml
  label: Domani Email API
  slug: domani-run-email-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domani-run/openapi/domani-run-email-api-openapi.yml
- filename: domani-run-mailzero-assistant-api-openapi.yml
  format: yaml
  label: Domani Mailzero Assistant API
  slug: domani-run-mailzero-assistant-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domani-run/openapi/domani-run-mailzero-assistant-api-openapi.yml
- filename: domani-run-marketplace-api-openapi.yml
  format: yaml
  label: Domani Marketplace API
  slug: domani-run-marketplace-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domani-run/openapi/domani-run-marketplace-api-openapi.yml
- filename: domani-run-notifications-api-openapi.yml
  format: yaml
  label: Domani Notifications API
  slug: domani-run-notifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domani-run/openapi/domani-run-notifications-api-openapi.yml
- filename: domani-run-referrals-api-openapi.yml
  format: yaml
  label: Domani Referrals API
  slug: domani-run-referrals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domani-run/openapi/domani-run-referrals-api-openapi.yml
- filename: domani-run-status-api-openapi.yml
  format: yaml
  label: Domani Status API
  slug: domani-run-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domani-run/openapi/domani-run-status-api-openapi.yml
- filename: domani-run-tlds-api-openapi.yml
  format: yaml
  label: Domani TLDs API
  slug: domani-run-tlds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domani-run/openapi/domani-run-tlds-api-openapi.yml
- filename: domani-run-verify-service-api-openapi.yml
  format: yaml
  label: Domani Verify Service API
  slug: domani-run-verify-service-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domani-run/openapi/domani-run-verify-service-api-openapi.yml
- filename: domani-run-webhooks-api-openapi.yml
  format: yaml
  label: Domani Webhooks API
  slug: domani-run-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domani-run/openapi/domani-run-webhooks-api-openapi.yml
auth_types: []
description: Authentication methods for Domani
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Domani Run Authentication
name_suffix: Authentication
oauth_flows: []
overview: Domani declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Domani
provider_slug: domani-run
scheme_count: 2
schemes:
- evidence: '"Authorization": "Bearer domani_sk_xxx"'
  header: Authorization
  location: header
  name: Bearer
  type: http-bearer
- authorize_url: https://domani.run/oauth/authorize
  evidence: '"authorization_endpoint":"https://domani.run/oauth/authorize"'
  flows:
  - authorization_code
  name: OAuth2
  scopes:
  - domains:read
  - domains:write
  - domains:transfer
  - tokens:read
  - tokens:write
  - webhooks:read
  - webhooks:write
  - email:read
  - email:write
  - email:delete
  - email:auth_secrets
  - email:manage_mailboxes
  - email:collaborate
  - workspace:read
  - workspace:write
  - account:read
  - account:write
  - billing:read
  - search
  - deals:read
  - deals:write
  - notifications:read
  - backorders:read
  - backorders:write
  - assistant:read
  - assistant:write
  type: oauth2
slug: domani-run-authentication
source_filename: domani-run-authentication.yml
source_heading: Authentication Profile
source_url: https://domani.run/.well-known/oauth-protected-resource
source_yaml: "generated: '2026-11-05'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://domani.run/.well-known/oauth-protected-resource\nsources:\n- https://domani.run/.well-known/oauth-protected-resource\n- https://domani.run/.well-known/oauth-authorization-server\n- https://dev.domani.run/setup\n- https://domani.run/en/setup\ndescription: Authentication methods for Domani\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: '\"Authorization\": \"Bearer domani_sk_xxx\"'\n  location: header\n  header: Authorization\n- type: oauth2\n  name: OAuth2\n  evidence: '\"authorization_endpoint\":\"https://domani.run/oauth/authorize\"'\n  flows:\n  - authorization_code\n  authorize_url: https://domani.run/oauth/authorize\n  scopes:\n  - domains:read\n  - domains:write\n  - domains:transfer\n  - tokens:read\n  - tokens:write\n  - webhooks:read\n  - webhooks:write\n  - email:read\n  - email:write\n  - email:delete\n  - email:auth_secrets\n  - email:manage_mailboxes\n\
  \  - email:collaborate\n  - workspace:read\n  - workspace:write\n  - account:read\n  - account:write\n  - billing:read\n  - search\n  - deals:read\n  - deals:write\n  - notifications:read\n  - backorders:read\n  - backorders:write\n  - assistant:read\n  - assistant:write\ndocs: https://domani.run/.well-known/oauth-protected-resource\n"
source_yaml_url: https://artifacts.apis.io/domani-run/authentication/domani-run-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Domain
- Email
- DNS
- Platform
---
