---
api_key_in:
- header
api_specs:
- filename: nhsd-developers-portal.postman_collection.json
  format: json
  label: NHSD FHIR API
  slug: nhsd-fhir-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/healthdirect/refs/heads/main/collections/nhsd-developers-portal.postman_collection.json
auth_types:
- oauth2
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Healthdirect Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Healthdirect Australia secures its APIs with oauth2 and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Healthdirect Australia
provider_slug: healthdirect
scheme_count: 2
schemes:
- flow: clientCredentials
  grant_params:
  - grant_type=client_credentials
  - client_id
  - client_secret
  name: oauth2ClientCredentials
  request_content_type: application/x-www-form-urlencoded
  scopes: []
  sources:
  - collections/nhsd-developers-portal.postman_collection.json
  tokenUrl: https://iam.int.nhsd.healthdirect.org.au/iam/oauth/token
  token_response_field: accessToken
  token_url_note: Integrator test environment; production IAM host mirrors this path.
  token_use: 'Sent as Authorization: Bearer <accessToken> on FHIR requests.'
  type: oauth2
- applies_to:
  - token request
  - all FHIR resource requests
  in: header
  name: apiKey
  parameter_name: x-api-key
  sources:
  - collections/nhsd-developers-portal.postman_collection.json
  type: apiKey
slug: healthdirect-authentication
source_filename: healthdirect-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: searched\nsource: collections/nhsd-developers-portal.postman_collection.json + NHSD Developer Guide\ndocs: https://about.healthdirect.gov.au/what-we-do/portfolio/nhsd/integration-hub/documentation\nsummary:\n  types: [oauth2, apiKey]\n  api_key_in: [header]\n  oauth2_flows: [clientCredentials]\n  note: >-\n    Dual credential model — every NHSD FHIR request carries BOTH an OAuth 2.0\n    bearer access token AND a static x-api-key header. This is a system-to-system\n    provider-directory API; there is no SMART-on-FHIR user/patient authorization\n    (no patient/*.read or system/*.rw scopes documented).\nschemes:\n- name: oauth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  tokenUrl: https://iam.int.nhsd.healthdirect.org.au/iam/oauth/token\n  token_url_note: Integrator test environment; production IAM host mirrors this path.\n  grant_params: [grant_type=client_credentials, client_id, client_secret]\n  request_content_type: application/x-www-form-urlencoded\n\
  \  token_response_field: accessToken\n  token_use: 'Sent as Authorization: Bearer <accessToken> on FHIR requests.'\n  scopes: []\n  sources: [collections/nhsd-developers-portal.postman_collection.json]\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter_name: x-api-key\n  applies_to: [token request, all FHIR resource requests]\n  sources: [collections/nhsd-developers-portal.postman_collection.json]\nonboarding:\n  gated: true\n  note: >-\n    Client credentials and API key are issued only after a formal onboarding —\n    a connection request for the Integrator Test Environment, production\n    registration, and an executed NHSD Agreement (~8 steps, ~3 months).\n  request_url: https://healthdirect-serviceline.atlassian.net/servicedesk/customer/portal/3/group/12/create/44\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/healthdirect/refs/heads/main/authentication/healthdirect-authentication.yml
summary_line: oauth2/apiKey · 2 schemes
tags:
- Healthcare
- Australia
- FHIR
- HL7
- Interoperability
- Provider Directory
- National Health System
- Health Services Directory
- Telehealth
- Digital Health
- Appointments
---
