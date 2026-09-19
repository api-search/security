---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: california-privacy-protection-agency-drop-data-broker-api-openapi.yml
  format: yaml
  label: DROP Data Broker API
  slug: drop-data-broker-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/california-privacy-protection-agency/refs/heads/main/openapi/california-privacy-protection-agency-drop-data-broker-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: California Privacy Protection Agency Authentication
name_suffix: Authentication
oauth_flows: []
overview: California Privacy Protection Agency secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: California Privacy Protection Agency
provider_slug: california-privacy-protection-agency
scheme_count: 1
schemes:
- applies_to: all operations (top-level security requirement, repeated per operation)
  description: API key issued through the Data Broker Portal. The key grants access only to the consumer deletion lists selected during setup.
  in: header
  name: ApiKeyAuth
  parameter: X-API-KEY
  sources:
  - openapi/california-privacy-protection-agency-drop-data-broker-api-openapi.yml
  - https://privacy.ca.gov/drop-for-data-brokers/technical-specifications/getting-started/
  type: apiKey
slug: california-privacy-protection-agency-authentication
source_filename: california-privacy-protection-agency-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: searched\nsource: openapi/california-privacy-protection-agency-drop-data-broker-api-openapi.yml\ndocs: https://privacy.ca.gov/drop-for-data-brokers/technical-specifications/getting-started/#authentication\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth: false\n  scopes: none\n  note: >-\n    Single static API key in the X-API-KEY header on every request. Keys are issued in the DROP Data\n    Broker Portal (https://databroker.drop.privacy.ca.gov/) only after the broker's account is\n    approved by CalPrivacy, registration or access fees are paid, and at least one consumer deletion\n    list is selected; the key is scoped to those selected lists. There is no OAuth, no scope\n    vocabulary, no self-serve developer sign-up: the credential is gated on the statutory\n    registration process, so an anonymous caller receives 401 and an unpaid or unregistered broker\n    receives 403.\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n\
  \  in: header\n  parameter: X-API-KEY\n  description: API key issued through the Data Broker Portal. The key grants access only to\n    the consumer deletion lists selected during setup.\n  applies_to: all operations (top-level security requirement, repeated per operation)\n  sources:\n  - openapi/california-privacy-protection-agency-drop-data-broker-api-openapi.yml\n  - https://privacy.ca.gov/drop-for-data-brokers/technical-specifications/getting-started/\nobtaining_credentials:\n  portal: https://databroker.drop.privacy.ca.gov/\n  steps:\n  - Sign in to the Data Broker Portal.\n  - Navigate to Home -> Consumer Deletion Lists and select the list(s) the business will process; click Save.\n  - Open the API Key tab and click \"Get a new API key\".\n  - For sandbox testing, navigate to SANDBOX ENVIRONMENT -> ISSUE SANDBOX API KEY.\n  prerequisites:\n  - DROP account created and approved by CalPrivacy (typically within two business days)\n  - Annual registration fee ($6,000 in 2026) or the\
  \ month-dependent access fee paid\n  - At least one consumer deletion list selected\nkey_rotation:\n  policy: >-\n    Regenerate the key if it is compromised or if the list selection changes. Issuing a new key\n    deactivates all previous keys (the \"API Key Changed\" notification says so).\n  storage_guidance: Store keys in environment variables or a secret management system.\ntransport:\n  tls: TLS 1.2+ required\nverification:\n  connectivity_check: GET https://api.drop.privacy.ca.gov/data/download with the X-API-KEY header; 200 confirms authentication\n  observed_anonymous_response:\n    url: https://api.drop.privacy.ca.gov/data/download\n    status: 401\n    body: API key is missing or invalid. Fix or regenerate the API key and try again.\n    probed: '2026-09-17'\nerrors:\n  '401': API key is missing or invalid — correct or regenerate the key\n  '403': Broker is not eligible — resolve account, registration, payment or access issue, or select at least one list\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/california-privacy-protection-agency/refs/heads/main/authentication/california-privacy-protection-agency-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Government
- Privacy
- Data Brokers
- Regulatory Compliance
- Data Deletion
- Consumer Rights
- California
- Webhook
---
