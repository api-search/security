---
api_key_in:
- header
api_specs:
- filename: galatea-bio-auth-api-openapi.yml
  format: yaml
  label: Galatea Bio Auth API
  slug: galatea-bio-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/galatea-bio/refs/heads/main/openapi/galatea-bio-auth-api-openapi.yml
- filename: galatea-bio-credit-api-openapi.yml
  format: yaml
  label: Galatea Bio Credit API
  slug: galatea-bio-credit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/galatea-bio/refs/heads/main/openapi/galatea-bio-credit-api-openapi.yml
- filename: galatea-bio-dashboard-api-openapi.yml
  format: yaml
  label: Galatea Bio Dashboard API
  slug: galatea-bio-dashboard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/galatea-bio/refs/heads/main/openapi/galatea-bio-dashboard-api-openapi.yml
- filename: galatea-bio-data-api-openapi.yml
  format: yaml
  label: Galatea Bio Data API
  slug: galatea-bio-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/galatea-bio/refs/heads/main/openapi/galatea-bio-data-api-openapi.yml
- filename: galatea-bio-exec-api-openapi.yml
  format: yaml
  label: Galatea Bio Exec API
  slug: galatea-bio-exec-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/galatea-bio/refs/heads/main/openapi/galatea-bio-exec-api-openapi.yml
- filename: galatea-bio-internal-api-openapi.yml
  format: yaml
  label: Galatea Bio Internal API
  slug: galatea-bio-internal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/galatea-bio/refs/heads/main/openapi/galatea-bio-internal-api-openapi.yml
- filename: galatea-bio-notification-api-openapi.yml
  format: yaml
  label: Galatea Bio Notification API
  slug: galatea-bio-notification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/galatea-bio/refs/heads/main/openapi/galatea-bio-notification-api-openapi.yml
- filename: galatea-bio-organizations-api-openapi.yml
  format: yaml
  label: Galatea Bio Organizations API
  slug: galatea-bio-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/galatea-bio/refs/heads/main/openapi/galatea-bio-organizations-api-openapi.yml
- filename: galatea-bio-statistics-api-openapi.yml
  format: yaml
  label: Galatea Bio Statistics API
  slug: galatea-bio-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/galatea-bio/refs/heads/main/openapi/galatea-bio-statistics-api-openapi.yml
- filename: galatea-bio-users-api-openapi.yml
  format: yaml
  label: Galatea Bio Users API
  slug: galatea-bio-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/galatea-bio/refs/heads/main/openapi/galatea-bio-users-api-openapi.yml
auth_types:
- apiKey
- http-bearer
description: ''
kind: authentication
layout: security
method: searched
name: Galatea Bio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Galatea Bio secures its APIs with apiKey and http-bearer across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Galatea Bio
provider_slug: galatea-bio
scheme_count: 1
schemes:
- applies_to: all operations (spec declares a global security requirement)
  format: 'JWT bearer token, sent as "Authorization: Bearer <access_token>"'
  in: header
  name: Bearer
  parameter: Authorization
  sources:
  - openapi/galatea-bio-octopod-openapi.yml
  type: apiKey
slug: galatea-bio-authentication
source_filename: galatea-bio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-16'\nmethod: searched\nsource: openapi/galatea-bio-octopod-openapi.yml\ndocs: https://docs.galatea.bio/#api-reference-auth-contents\nnote: >-\n  Derived from the published Octopod API Swagger 2.0 document, then upgraded from the GalateaBio\n  Ancestry API documentation and the first-party octopod-cli client. The spec declares a single\n  security definition (apiKey named \"Authorization\" in header) which the docs and client confirm\n  carries a JWT bearer token in the form \"Authorization: Bearer <token>\".\nsummary:\n  types:\n  - apiKey\n  - http-bearer\n  api_key_in:\n  - header\n  oauth2_flows: []\n  mfa: true\n  applied_globally: true\nschemes:\n- name: Bearer\n  type: apiKey\n  in: header\n  parameter: Authorization\n  format: 'JWT bearer token, sent as \"Authorization: Bearer <access_token>\"'\n  sources:\n  - openapi/galatea-bio-octopod-openapi.yml\n  applies_to: all operations (spec declares a global security requirement)\ncredential_modes:\n-\
  \ mode: organization API key\n  description: >-\n    A long-lived organization API key minted by an organization admin. Used directly as the bearer\n    token. The octopod-cli calls this api_mode=1.\n  issued_by: POST /organizations/{organization_id}/generate-api-key\n  operation_id: organizations_generate-api-key_create\n  docs: https://docs.galatea.bio/#recipe-authentication\n- mode: username and password login\n  description: >-\n    Email + password exchanged for a short-lived access token, a refresh token, and a websocket\n    access token. The docs explicitly warn the fetched access token has a short lifetime. The\n    octopod-cli calls this api_mode=2.\n  issued_by: POST /users/auth\n  operation_id: users_auth_create\n  request_fields: [email, password]\n  response_fields: [access, refresh, websocket_access]\n  docs: https://docs.galatea.bio/#api-reference-auth-login\n- mode: SFTP key-based\n  description: >-\n    Separate credential path for bulk file transfer. Organizations manage\
  \ SFTP users and their SSH\n    public keys through the API; uploads then authenticate to the SFTP host with a private keyfile\n    rather than a bearer token.\n  issued_by: POST /organizations/{organization_id}/sftp_users/{sftp_user_id}/ssh_keys\n  operation_id: organizations_sftp_users_ssh_keys_create\n  docs: https://docs.galatea.bio/#recipe-upload-file-with-sftp-get-status\ntoken_lifecycle:\n- action: obtain\n  operation_id: users_auth_create\n  path: POST /users/auth\n- action: multi-factor confirmation\n  operation_id: users_confirm_create\n  path: POST /users/confirm\n  note: Requires mfa_session_id plus a numeric code; MFA is part of the published login flow.\n- action: request a new MFA code\n  operation_id: users_request-new-code_create\n  path: POST /users/request-new-code\n- action: refresh\n  operation_id: users_refresh_create\n  path: POST /users/refresh\n  note: Takes both the refresh token and the expired access token.\n- action: revoke\n  operation_id: users_logout_create\n\
  \  path: POST /users/logout\n  note: Requires the refresh token; returns HTTP 200 on successful logout.\npassword_management:\n- operation_id: users_change-password_create\n  path: POST /users/change-password\n- operation_id: users_forgot-password_create\n  path: POST /users/forgot-password\n- operation_id: users_reset-password_create\n  path: POST /users/reset-password\n- operation_id: users_activate_create\n  path: POST /users/activate\nwebhook_authentication:\n  scheme: HMAC-SHA256 signature, base64 encoded\n  header: X-Octopod-Signature\n  signed_payload: sender_host + raw request body\n  secret_issued_by: POST /organizations/{organization_id}/generate-webhooks-secret\n  docs: https://docs.galatea.bio/#recipe-handling-webhooks-deliveries\n  see: asyncapi/galatea-bio-octopod-webhooks.yml\nenvironments:\n- name: production\n  base_url: https://api.galatea.bio/api/v1\n  webhook_sender_host: api.galatea.bio\n- name: sandbox\n  base_url: https://api.sandbox.galatea.bio/api/v1\n  webhook_sender_host:\
  \ api.sandbox.galatea.bio\nunauthenticated_response:\n  status: 401\n  body: '{\"detail\": \"Authentication credentials were not provided.\"}'\n  observed: 'GET https://api.galatea.bio/api/v1/users/me on 2026-08-16'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/galatea-bio/refs/heads/main/authentication/galatea-bio-authentication.yml
summary_line: apiKey/http-bearer · 1 scheme
tags:
- Genomics
- Bioinformatics
- Ancestry
- Precision Medicine
- polygenic-risk-score
- Clinical Laboratory
- Genetic Testing
- Biobank
- Life Sciences
- Health
- Sequencing
---
