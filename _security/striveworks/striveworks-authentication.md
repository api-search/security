---
api_key_in: []
auth_types:
- oauth2
- http
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Striveworks Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Striveworks secures its APIs with oauth2, http, and mutualTLS across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Striveworks
provider_slug: striveworks
scheme_count: 3
schemes:
- credential_lifetime: Client credentials are created from the user's Profile page with a name and an expiration date of up to one year from the date of creation.
  flow: clientCredentials
  grant_type: client_credentials
  name: client_credentials
  request_content_type: application/x-www-form-urlencoded
  request_parameters:
  - client_id
  - client_secret
  - grant_type
  response_fields:
  - access_token
  - expires_in
  source: https://production.chariot.striveworks.us/docs/user_guide/administration/authentication
  token_url: https://<chariot_url>/auth/client/v2/chariot/login
  type: oauth2
- description: Bearer token returned by the client-credentials login endpoint; required on all subsequent requests to the Chariot REST API.
  format: 'Authorization: Bearer <access_token>'
  in: header
  name: bearer
  parameter: Authorization
  scheme: bearer
  source: https://production.chariot.striveworks.us/docs/user_guide/administration/authentication
  type: http
- description: PKI / client-certificate authentication for environments that require it. Supported via PKCS#12 bundle (pkcs12 + pkcs12_password) or separate certificate and key files (cert_filename, key_filename), both through the SDK connect() call and directly with an HTTP client. Can be combined with a bearer token.
  name: pki
  source: https://production.chariot.striveworks.us/docs/user_guide/administration/authentication
  type: mutualTLS
slug: striveworks-authentication
source_filename: striveworks-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: searched\nsource: https://production.chariot.striveworks.us/docs/user_guide/administration/authentication\ndocs: https://production.chariot.striveworks.us/docs/user_guide/administration/authentication\nsummary:\n  types: [oauth2, http, mutualTLS]\n  oauth2_flows: [clientCredentials]\n  bearer_token: true\n  api_key_in: []\n  notes: >-\n    Chariot is deployed per tenant, so every authentication URL below is relative to the customer's own\n    Chariot host (the docs write it as https://<chariot_url>). The Striveworks-operated instance used for\n    these probes is https://production.chariot.striveworks.us. There is no published OpenAPI declaring\n    securitySchemes, so this profile is captured from the provider's authentication documentation rather\n    than derived from a spec.\nschemes:\n  - name: client_credentials\n    type: oauth2\n    flow: clientCredentials\n    token_url: https://<chariot_url>/auth/client/v2/chariot/login\n    grant_type:\
  \ client_credentials\n    request_content_type: application/x-www-form-urlencoded\n    request_parameters: [client_id, client_secret, grant_type]\n    response_fields: [access_token, expires_in]\n    credential_lifetime: >-\n      Client credentials are created from the user's Profile page with a name and an expiration date of\n      up to one year from the date of creation.\n    source: https://production.chariot.striveworks.us/docs/user_guide/administration/authentication\n  - name: bearer\n    type: http\n    scheme: bearer\n    in: header\n    parameter: Authorization\n    format: 'Authorization: Bearer <access_token>'\n    description: >-\n      Bearer token returned by the client-credentials login endpoint; required on all subsequent\n      requests to the Chariot REST API.\n    source: https://production.chariot.striveworks.us/docs/user_guide/administration/authentication\n  - name: pki\n    type: mutualTLS\n    description: >-\n      PKI / client-certificate authentication for\
  \ environments that require it. Supported via PKCS#12\n      bundle (pkcs12 + pkcs12_password) or separate certificate and key files (cert_filename,\n      key_filename), both through the SDK connect() call and directly with an HTTP client. Can be\n      combined with a bearer token.\n    source: https://production.chariot.striveworks.us/docs/user_guide/administration/authentication\nsdk_helpers:\n  - language: python\n    package: chariot-client\n    function: chariot.client.connect\n    modes: [client_id + client_secret, bearer_token, pkcs12, cert_filename + key_filename]\n  - language: cli\n    command: chariot init\n    modes: ['--credentials credentials.json', interactive]\nauthorization_model:\n  style: rbac\n  docs: https://production.chariot.striveworks.us/docs/user_guide/administration/roles-permissions\n  note: >-\n    Authorization is role-based over organizations and projects rather than OAuth scopes; no scope\n    strings are issued with the access token, so no scopes/ artifact\
  \ is emitted for this provider.\n  organization_roles:\n    - name: Organization Owner\n      description: Complete administrative control of the organization and all its contents; inherits project Owner permissions for every project in the organization.\n    - name: Organization Maintainer\n      description: Can add and remove users in the organization; cannot view private projects they are not a member of and cannot add or remove organization Owners.\n    - name: Organization Contributor\n      description: Member of the organization with read and write access to projects based on project visibility and membership; no organization-level administration.\n  project_roles:\n    - name: Project Owner\n      description: Complete administrative control over the project.\n    - name: Project Writer\n      description: Can create and edit resources (datasets, models, and similar) within the project.\n    - name: Project Reader\n      description: Can view all project contents but cannot make\
  \ edits.\n  permissions:\n    - {resource: org, permission: org_read}\n    - {resource: org, permission: add_owner}\n    - {resource: org, permission: remove_owner}\n    - {resource: org, permission: org_update_settings}\n    - {resource: org, permission: add_user}\n    - {resource: org, permission: remove_user}\n    - {resource: org, permission: project_create}\n    - {resource: project, permission: project_read}\n    - {resource: project, permission: project_write}\n    - {resource: project, permission: project_delete}\n    - {resource: project, permission: project_update_settings}\n    - {resource: project, permission: add_owner}\n    - {resource: project, permission: remove_owner}\n    - {resource: project, permission: add_user}\n    - {resource: project, permission: remove_user}\n    - {resource: project, permission: secret_write}\n    - {resource: project, permission: secret_decrypt}\n    - {resource: project, permission: secret_list}\n    - {resource: project, permission: dataset_read}\n\
  \    - {resource: project, permission: dataset_create}\n    - {resource: project, permission: dataset_write}\n    - {resource: project, permission: training_job_read}\n    - {resource: project, permission: training_job_create}\n    - {resource: project, permission: training_job_write}\n    - {resource: project, permission: annotation_task_read}\n    - {resource: project, permission: annotation_task_create}\n    - {resource: project, permission: annotation_task_write}\n    - {resource: project, permission: model_read}\n    - {resource: project, permission: model_create}\n    - {resource: project, permission: model_write}\n    - {resource: project, permission: inference_server_read}\n    - {resource: project, permission: inference_server_create}\n    - {resource: project, permission: inference_server_write}\n    - {resource: project, permission: workspace_read}\n    - {resource: project, permission: workspace_create}\n    - {resource: project, permission: workspace_write}\n  visibility_modifiers:\
  \ [public, restricted, internal, private]\nx-evidence:\n  - {fetched: '2026-08-05', url: 'https://production.chariot.striveworks.us/docs/user_guide/administration/authentication', http_status: 200}\n  - {fetched: '2026-08-05', url: 'https://production.chariot.striveworks.us/docs/user_guide/administration/roles-permissions', http_status: 200}\n  - {fetched: '2026-08-05', url: 'https://production.chariot.striveworks.us/api/identity/v2/users/me/', http_status: 401, body: '{\"error\":\"invalid bearer token\"}'}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/striveworks/refs/heads/main/authentication/striveworks-authentication.yml
summary_line: oauth2/http/mutualTLS · 3 schemes
tags:
- Company
- Artificial Intelligence
- Machine-Learning
- MLOps
- AIOps
- Model Deployment
- Model Monitoring
- Inference
- Data Annotation
- Computer-Vision
- Agentic Workflows
- Defense
- GovTech
- Edge Computing
---
