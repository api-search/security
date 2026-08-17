---
api_key_in:
- header
api_specs:
- filename: workramp-api-settings-openapi.yml
  format: yaml
  label: WorkRamp API
  slug: workramp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workramp/refs/heads/main/openapi/workramp-api-settings-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Workramp Authentication
name_suffix: Authentication
oauth_flows: []
overview: WorkRamp secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: WorkRamp
provider_slug: workramp
scheme_count: 1
schemes:
- format: Bearer <api_key>
  in: header
  name: sec0
  note: 'Declared in the contract as apiKey-in-header with x-bearer-format "bearer", i.e. the key is sent as `Authorization: Bearer <key>` even though it is a static API key and not an OAuth token.'
  parameter: Authorization
  sources:
  - openapi/workramp-api-settings-openapi.yml
  - openapi/workramp-json-api-openapi.yml
  type: apiKey
slug: workramp-authentication
source_filename: workramp-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/workramp-api-settings-openapi.yml, openapi/workramp-json-api-openapi.yml\ndocs: https://developers.workramp.com/reference/basic-auth\nkey_management_docs: https://help.workramp.com/en/articles/9574489-api-key-management\nsummary:\n  types:\n    - apiKey\n  api_key_in:\n    - header\n  oauth2_flows: []\n  oauth: false\n  openid_connect: false\n  mtls: false\nschemes:\n  - name: sec0\n    type: apiKey\n    in: header\n    parameter: Authorization\n    format: 'Bearer <api_key>'\n    sources:\n      - openapi/workramp-api-settings-openapi.yml\n      - openapi/workramp-json-api-openapi.yml\n    note: >-\n      Declared in the contract as apiKey-in-header with x-bearer-format \"bearer\", i.e. the\n      key is sent as `Authorization: Bearer <key>` even though it is a static API key and\n      not an OAuth token.\nexample: |\n  curl https://app.workramp.com/api/v1/users \\\n    -H \"Authorization: Bearer YOUR_API_KEY_HERE\"\
  \nkey_model:\n  issuance: >-\n    Any admin generates keys on the in-app Integrations page -> API\n    (https://<subdomain>.app.workramp.com/admin/integrations/access-token). A description\n    documenting the key's intended use is required at creation.\n  ownership: >-\n    Every key belongs to a specific user, who must be an admin. Actions taken with the key\n    are attributed to that user — assign a training with a key and the assigner is the key\n    owner.\n  scopes: none\n  permission_model: >-\n    Inherited from the owning admin user. There is no scope, role or least-privilege\n    surface: the docs state plainly that \"anyone with your API token is able to read any\n    information, including private user information, and to make any changes in your\n    organization's Learn:Up account.\"\n  cardinality: unlimited keys per admin or service account\n  service_accounts: >-\n    Recommended pattern — create a dedicated non-human admin (\"Automation Account\") to own\n    integration\
  \ keys, because a key stops working when its owning user is deactivated.\n  visibility: >-\n    Shown once at creation. Once the modal is dismissed the key cannot be viewed or copied\n    again in WorkRamp.\n  rotation: Keys can be refreshed (regenerated) or deleted from the admin key table at any time.\n  revocation: Immediate on delete; an automated email goes to the key owner on create, refresh or delete.\n  expiry: none published\n  prefix: none published\n  scoping_across_clouds: One key works for both the Employee Learning Cloud and the Customer Learning Cloud.\nprovisioning:\n  scim:\n    version: '2.0'\n    endpoints:\n      - /scim/v2/Users\n      - /scim/v2/Users/{id}\n      - /scim/v2/Groups\n      - /scim/v2/Groups/{id}\n    source: openapi/workramp-api-settings-openapi.yml\n    auth: same Authorization bearer API key as the REST API\n  sso:\n    supported: true\n    note: >-\n      SSO/SCIM identities surface on the user object as userIdentifiers with namespace\n      \"sso_scim\"\
  ; the API also exposes /api/v1/instant_auth and\n      /api/v1/academies/{academy_id}/instant_auth_request for signing a known user straight\n      into a session.\naccess_gate:\n  public: false\n  statement: >-\n    \"This is a private API. Contact support@workramp.com to see if you are eligible, and\n    request access.\" An enterprise account provisioned for Learn:Up is a prerequisite.\n  source: https://developers.workramp.com/reference/getting-started\nregions:\n  - host: https://app.workramp.com\n    default: true\n  - host: https://app.eu.workramp.com\n    note: EU customers substitute this host in all API URLs; the auth model is identical.\ngaps:\n  - No OAuth 2.0 or OpenID Connect for third-party app authorization — only long-lived admin-scoped API keys.\n  - No scopes, no least-privilege key restriction, no key expiry.\n  - Key compromise is a full-tenant compromise; the docs say so explicitly.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workramp/refs/heads/main/authentication/workramp-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Learning Management
- Revenue Enablement
- Sales Enablement
- Training
- Onboarding
- LMS
- Assessments
- Certifications
- Coaching
- Go-to-Market
- SCIM
- SCORM
- Webhooks
- Customer Education
---
