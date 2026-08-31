---
api_key_in:
- header
api_specs:
- filename: osano-cmp-api-openapi.yml
  format: yaml
  label: Osano Cmp API
  slug: osano-cmp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/osano/refs/heads/main/openapi/osano-cmp-api-openapi.yml
- filename: osano-cmprules-api-openapi.yml
  format: yaml
  label: Osano Cmp Rules API
  slug: osano-cmprules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/osano/refs/heads/main/openapi/osano-cmprules-api-openapi.yml
- filename: osano-collections-api-openapi.yml
  format: yaml
  label: Osano Collections API
  slug: osano-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/osano/refs/heads/main/openapi/osano-collections-api-openapi.yml
- filename: osano-config-api-openapi.yml
  format: yaml
  label: Osano Config API
  slug: osano-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/osano/refs/heads/main/openapi/osano-config-api-openapi.yml
- filename: osano-connectors-api-openapi.yml
  format: yaml
  label: Osano Connectors API
  slug: osano-connectors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/osano/refs/heads/main/openapi/osano-connectors-api-openapi.yml
- filename: osano-consent-profiles-api-openapi.yml
  format: yaml
  label: Osano Consent Profiles API
  slug: osano-consent-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/osano/refs/heads/main/openapi/osano-consent-profiles-api-openapi.yml
- filename: osano-consents-api-openapi.yml
  format: yaml
  label: Osano Consents API
  slug: osano-consents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/osano/refs/heads/main/openapi/osano-consents-api-openapi.yml
- filename: osano-customerinsights-api-openapi.yml
  format: yaml
  label: Osano Customer Insights API
  slug: osano-customerinsights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/osano/refs/heads/main/openapi/osano-customerinsights-api-openapi.yml
- filename: osano-datadiscovery-api-openapi.yml
  format: yaml
  label: Osano Data Discovery API
  slug: osano-datadiscovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/osano/refs/heads/main/openapi/osano-datadiscovery-api-openapi.yml
- filename: osano-dsar-api-openapi.yml
  format: yaml
  label: Osano Dsar API
  slug: osano-dsar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/osano/refs/heads/main/openapi/osano-dsar-api-openapi.yml
- filename: osano-dsaractionitems-api-openapi.yml
  format: yaml
  label: Osano Dsar Action Items API
  slug: osano-dsaractionitems-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/osano/refs/heads/main/openapi/osano-dsaractionitems-api-openapi.yml
- filename: osano-sessions-api-openapi.yml
  format: yaml
  label: Osano Sessions API
  slug: osano-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/osano/refs/heads/main/openapi/osano-sessions-api-openapi.yml
- filename: osano-subjectrightsportal-api-openapi.yml
  format: yaml
  label: Osano Subject Rights Portal API
  slug: osano-subjectrightsportal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/osano/refs/heads/main/openapi/osano-subjectrightsportal-api-openapi.yml
- filename: osano-subjects-api-openapi.yml
  format: yaml
  label: Osano Subjects API
  slug: osano-subjects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/osano/refs/heads/main/openapi/osano-subjects-api-openapi.yml
- filename: osano-token-api-openapi.yml
  format: yaml
  label: Osano Token API
  slug: osano-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/osano/refs/heads/main/openapi/osano-token-api-openapi.yml
- filename: osano-unified-consent-core-api-api-openapi.yml
  format: yaml
  label: Osano Unified Consent Core API
  slug: osano-unified-consent-core-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/osano/refs/heads/main/openapi/osano-unified-consent-core-api-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Osano Authentication
name_suffix: Authentication
oauth_flows: []
overview: Osano secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Osano
provider_slug: osano
scheme_count: 2
schemes:
- applies_to:
  - api: Osano Customer REST API
    scope: All 43 operations.
  - api: Osano Unified Consent Core API
    scope: '"Routes that involve creating, updating, or merging subjects require the Osano API key."'
  display_name: Osano API key
  expiry: Keys are described as needing to be "valid, unexpired" — an expiry exists but no lifetime is published.
  in: header
  issued_at: https://my.osano.com/api-keys
  name: ApiKeyAuth
  parameter: x-osano-api-key
  requires_privilege: '"You must be an admin or have the correct privileges to generate an API key."'
  sources:
  - openapi/osano-customer-rest-api-openapi.yml
  - openapi/osano-unified-consent-core-api-openapi.yml
  type: apiKey
- applies_to:
  - api: Osano Unified Consent Core API
    scope: '"All other routes require the Unified Consent API key" — i.e. everything except subject create/update/merge.'
  browser_safe: The UC JS SDK is documented as taking a `token` and `apiUrl` to "return a UnifiedConsentByOsano Client with the ability to submit consents, but not manage subjects, which is suitable for use in a browser environment" — so the UC key/token is the constrained credential by design.
  description: Unified Consent API key
  display_name: Unified Consent API key
  in: header
  name: ucApiKey
  parameter: x-uc-api-key
  sources:
  - openapi/osano-unified-consent-core-api-openapi.yml
  type: apiKey
slug: osano-authentication
source_filename: osano-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: openapi/osano-customer-rest-api-openapi.yml, openapi/osano-unified-consent-core-api-openapi.yml\ndocs:\n- https://developers.osano.com/customer-rest-api/developer-api-doc\n- https://developers.osano.com/uc/core-api/openapi\n- https://my.osano.com/api-keys\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n  http_basic: false\n  http_bearer: false\nnote: >-\n  Both Osano APIs authenticate with a long-lived API key in a custom header. There is no OAuth 2.0,\n  no OpenID Connect, no bearer token and no mTLS on either surface, and no scopes of any kind — a key\n  carries whatever privileges its issuing user has, account-wide. The Unified Consent Core API is the\n  interesting case: it uses TWO different keys against the SAME host and the choice is\n  route-dependent rather than declared per-operation in the spec (the spec sets a blanket\n  `security: [{ ucApiKey:\
  \ [] }]`), so an integrator must read the prose to know which key a route\n  wants. Getting a key is also not fully self-serve — Osano's FAQ says \"Open a ticket with support to\n  enable API access if you are on a tier that includes API access.\"\n  Neither spec documents a 401 or 403 response on any operation.\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-osano-api-key\n  display_name: Osano API key\n  issued_at: https://my.osano.com/api-keys\n  requires_privilege: >-\n    \"You must be an admin or have the correct privileges to generate an API key.\"\n  applies_to:\n  - api: Osano Customer REST API\n    scope: All 43 operations.\n  - api: Osano Unified Consent Core API\n    scope: >-\n      \"Routes that involve creating, updating, or merging subjects require the Osano API key.\"\n  expiry: >-\n    Keys are described as needing to be \"valid, unexpired\" — an expiry exists but no lifetime is\n    published.\n  sources:\n  - openapi/osano-customer-rest-api-openapi.yml\n\
  \  - openapi/osano-unified-consent-core-api-openapi.yml\n- name: ucApiKey\n  type: apiKey\n  in: header\n  parameter: x-uc-api-key\n  display_name: Unified Consent API key\n  description: Unified Consent API key\n  applies_to:\n  - api: Osano Unified Consent Core API\n    scope: >-\n      \"All other routes require the Unified Consent API key\" — i.e. everything except subject\n      create/update/merge.\n  browser_safe: >-\n    The UC JS SDK is documented as taking a `token` and `apiUrl` to \"return a UnifiedConsentByOsano\n    Client with the ability to submit consents, but not manage subjects, which is suitable for use in\n    a browser environment\" — so the UC key/token is the constrained credential by design.\n  sources:\n  - openapi/osano-unified-consent-core-api-openapi.yml\nexample_verbatim:\n  customer_rest_api: \"curl --header 'x-osano-api-key: myapikey' https://api.osano.com/v1/data-stores\"\n  unified_consent: \"curl --header 'x-uc-api-key: <API_KEY>' https://uc.api.osano.com/v2/consents/check/some-subject-id\"\
  \nscopes:\n  published: false\n  note: >-\n    No OAuth scopes and no API-key permission scopes are published. See scopes/ — no artifact was\n    written because there is nothing to derive.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/osano/refs/heads/main/authentication/osano-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Data Privacy
- Consent Management
- Compliance
- GDPR
- CCPA
- Cookie Consent
- Subject Rights
- Data Mapping
- Vendor Risk
- Privacy Assessments
- Governance Risk Compliance
---
