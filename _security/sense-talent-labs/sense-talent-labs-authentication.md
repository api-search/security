---
api_key_in: []
api_specs:
- filename: sense-talent-labs-appointment-api-openapi.yml
  format: yaml
  label: Sense Talent Labs Appointment API
  slug: sense-talent-labs-appointment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sense-talent-labs/refs/heads/main/openapi/sense-talent-labs-appointment-api-openapi.yml
- filename: sense-talent-labs-authentication-api-openapi.yml
  format: yaml
  label: Sense Talent Labs Authentication API
  slug: sense-talent-labs-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sense-talent-labs/refs/heads/main/openapi/sense-talent-labs-authentication-api-openapi.yml
- filename: sense-talent-labs-candidate-api-openapi.yml
  format: yaml
  label: Sense Talent Labs Candidate API
  slug: sense-talent-labs-candidate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sense-talent-labs/refs/heads/main/openapi/sense-talent-labs-candidate-api-openapi.yml
- filename: sense-talent-labs-certification-api-openapi.yml
  format: yaml
  label: Sense Talent Labs Certification API
  slug: sense-talent-labs-certification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sense-talent-labs/refs/heads/main/openapi/sense-talent-labs-certification-api-openapi.yml
- filename: sense-talent-labs-clientcontact-api-openapi.yml
  format: yaml
  label: Sense Talent Labs Client Contact API
  slug: sense-talent-labs-clientcontact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sense-talent-labs/refs/heads/main/openapi/sense-talent-labs-clientcontact-api-openapi.yml
- filename: sense-talent-labs-company-api-openapi.yml
  format: yaml
  label: Sense Talent Labs Company API
  slug: sense-talent-labs-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sense-talent-labs/refs/heads/main/openapi/sense-talent-labs-company-api-openapi.yml
- filename: sense-talent-labs-internaluser-api-openapi.yml
  format: yaml
  label: Sense Talent Labs Internal User API
  slug: sense-talent-labs-internaluser-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sense-talent-labs/refs/heads/main/openapi/sense-talent-labs-internaluser-api-openapi.yml
- filename: sense-talent-labs-joborder-api-openapi.yml
  format: yaml
  label: Sense Talent Labs Job Order API
  slug: sense-talent-labs-joborder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sense-talent-labs/refs/heads/main/openapi/sense-talent-labs-joborder-api-openapi.yml
- filename: sense-talent-labs-lead-api-openapi.yml
  format: yaml
  label: Sense Talent Labs Lead API
  slug: sense-talent-labs-lead-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sense-talent-labs/refs/heads/main/openapi/sense-talent-labs-lead-api-openapi.yml
- filename: sense-talent-labs-placement-api-openapi.yml
  format: yaml
  label: Sense Talent Labs Placement API
  slug: sense-talent-labs-placement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sense-talent-labs/refs/heads/main/openapi/sense-talent-labs-placement-api-openapi.yml
- filename: sense-talent-labs-submission-api-openapi.yml
  format: yaml
  label: Sense Talent Labs Submission API
  slug: sense-talent-labs-submission-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sense-talent-labs/refs/heads/main/openapi/sense-talent-labs-submission-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Sense Talent Labs Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Sense Talent Labs secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Sense Talent Labs
provider_slug: sense-talent-labs
scheme_count: 2
schemes:
- flows:
  - flow: clientCredentials
    grant_types:
    - client_credentials
    scopes: 1
    tokenUrl: https://partner-auth.us-stage.sensehq.co/oauth2/token
    tokenUrl_note: The securitySchemes block in the published OpenAPI declares the STAGE token endpoint (partner-auth.us-stage.sensehq.co). The production token endpoint (partner-auth.sensehq.com/oauth2/token) is the one used in every sample-code block in the same document's info.description. Recorded as published; not corrected in the spec.
    tokenUrl_production: https://partner-auth.sensehq.com/oauth2/token
  name: sense_authentication
  sources:
  - openapi/sense-talent-labs-sense-api-openapi.json
  - https://developer.sensehq.com/
  type: oauth2
- applied: default security for every operation except POST /oauth2/token
  bearerFormat: JWT
  name: sense_bearer_auth
  scheme: bearer
  sources:
  - openapi/sense-talent-labs-sense-api-openapi.json
  type: http
slug: sense-talent-labs-authentication
source_filename: sense-talent-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: https://developer.sensehq.com/\ndocs: https://developer.sensehq.com/\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\n  model: OAuth 2.0 client credentials exchanged for a short-lived bearer JWT; no scopes.\n  credential_issuance: manual — \"The Sense Team will provide you with credentials that will\n    synchronize data to your account at your-agency-name.sensehq.com.\" There is no self-serve\n    key or client registration surface.\nschemes:\n- name: sense_authentication\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://partner-auth.us-stage.sensehq.co/oauth2/token\n    tokenUrl_production: https://partner-auth.sensehq.com/oauth2/token\n    tokenUrl_note: The securitySchemes block in the published OpenAPI declares the STAGE token\n      endpoint (partner-auth.us-stage.sensehq.co). The production token endpoint\n      (partner-auth.sensehq.com/oauth2/token) is the\
  \ one used in every sample-code block in the\n      same document's info.description. Recorded as published; not corrected in the spec.\n    scopes: 1\n    grant_types:\n    - client_credentials\n  sources:\n  - openapi/sense-talent-labs-sense-api-openapi.json\n  - https://developer.sensehq.com/\n- name: sense_bearer_auth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  applied: default security for every operation except POST /oauth2/token\n  sources:\n  - openapi/sense-talent-labs-sense-api-openapi.json\ntoken:\n  lifetime_seconds: 300\n  lifetime_source: expires_in field in the token response\n  caching_required: true\n  caching_policy: 'Clients MUST cache and reuse access tokens until they expire. The docs\n    explicitly warn against hardcoding the 300-second lifetime because it may change without\n    notice, and state that unnecessary token requests \"may lead to rate limiting or\n    deactivation.\"'\n  response_fields:\n  - access_token\n  - expires_in\n  - token_type\n\
  request:\n  header: 'Authorization: Bearer <access_token>'\n  token_request_content_type: application/x-www-form-urlencoded\n  token_request_fields:\n  - client_id\n  - client_secret\n  - grant_type\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sense-talent-labs/refs/heads/main/authentication/sense-talent-labs-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Human Resources
- Recruiting
- Talent Acquisition
- Staffing
- Applicant Tracking
- Candidate Engagement
- Recruiting Automation
- Talent CRM
- Messaging
- Interview Scheduling
- Artificial Intelligence
- SaaS
---
