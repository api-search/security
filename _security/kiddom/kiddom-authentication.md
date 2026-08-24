---
api_key_in: []
auth_types:
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Kiddom Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kiddom secures its APIs with openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Kiddom
provider_slug: kiddom
scheme_count: 3
schemes:
- detail: An LMS platform initiates the launch; Kiddom validates the platform's signed id_token against the platform's JWKS and the deployment registration. Kiddom's own tool key set, client_id and deployment_id are provisioned per district by Kiddom support and are NOT published — no /lti/jwks, /jwks.json or /.well-known/lti-configuration is served (all 404 on api.kiddom.co).
  endpoints:
    launch: https://api.kiddom.co/lti/launch
    login: https://api.kiddom.co/lti/login
  name: LTI 1.3 OIDC third-party-initiated login
  role: tool
  services:
  - Assignment and Grade Services 2.0 (grade passback to the LMS gradebook)
  - Names and Role Provisioning Services 2.0
  - Deep Linking 2.0
  source: https://site.imsglobal.org/certifications/kiddom-inc/kiddom
  type: openIdConnect
- detail: End users sign in at https://app.kiddom.co/login through the district's SSO provider. Clever and ClassLink also drive automated rostering; per the help center, neither supports grade passback to an LMS, which requires rostering through the LMS itself.
  name: SSO via rostering provider
  providers:
  - Clever
  - ClassLink
  - Google Classroom
  - Canvas
  - Schoology
  - Microsoft Teams
  source: https://get.kiddom.co/rostering-and-integrations/
  type: federated
- detail: 'Fallback for districts without an SSO/rostering integration: manual accounts, CSV bulk upload, class codes.'
  name: Manual accounts and class codes
  source: https://support.kiddom.co/en/articles/14724758-where-is-my-class-code
  type: password
slug: kiddom-authentication
source_filename: kiddom-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: searched\nsource: https://support.kiddom.co/en/collections/19663428-rostering-and-integrations\ndocs: https://get.kiddom.co/rostering-and-integrations/\nnote: >-\n  Nothing here is derived from a spec — Kiddom publishes no OpenAPI, so derive-authentication.py\n  has no input. This profile is assembled from the 1EdTech certification record, the help center's\n  integration articles, and live probes. There is no API key, no developer signup, and no token\n  endpoint: authentication into Kiddom is federated from the district's identity/rostering\n  provider, and machine-to-machine authentication happens inside the LTI 1.3 launch.\nsummary:\n  types:\n  - openIdConnect\n  api_key_in: []\n  oauth2_flows: []\n  developer_credentials: none-published\nschemes:\n- name: LTI 1.3 OIDC third-party-initiated login\n  type: openIdConnect\n  role: tool\n  source: https://site.imsglobal.org/certifications/kiddom-inc/kiddom\n  endpoints:\n    login: https://api.kiddom.co/lti/login\n\
  \    launch: https://api.kiddom.co/lti/launch\n  detail: >-\n    An LMS platform initiates the launch; Kiddom validates the platform's signed id_token against\n    the platform's JWKS and the deployment registration. Kiddom's own tool key set, client_id and\n    deployment_id are provisioned per district by Kiddom support and are NOT published — no\n    /lti/jwks, /jwks.json or /.well-known/lti-configuration is served (all 404 on api.kiddom.co).\n  services:\n  - Assignment and Grade Services 2.0 (grade passback to the LMS gradebook)\n  - Names and Role Provisioning Services 2.0\n  - Deep Linking 2.0\n- name: SSO via rostering provider\n  type: federated\n  providers:\n  - Clever\n  - ClassLink\n  - Google Classroom\n  - Canvas\n  - Schoology\n  - Microsoft Teams\n  source: https://get.kiddom.co/rostering-and-integrations/\n  detail: >-\n    End users sign in at https://app.kiddom.co/login through the district's SSO provider. Clever\n    and ClassLink also drive automated rostering; per\
  \ the help center, neither supports grade\n    passback to an LMS, which requires rostering through the LMS itself.\n- name: Manual accounts and class codes\n  type: password\n  source: https://support.kiddom.co/en/articles/14724758-where-is-my-class-code\n  detail: 'Fallback for districts without an SSO/rostering integration: manual accounts, CSV bulk upload, class codes.'\nabsent:\n- api_keys: 'No API key issuance, developer portal, or key management surface exists.'\n- oauth2: '/oauth/token and /oauth/authorize return 404 on api.kiddom.co.'\n- oidc_discovery: '/.well-known/openid-configuration returns 404 on every Kiddom host.'\n- mtls: 'Not documented.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kiddom/refs/heads/main/authentication/kiddom-authentication.yml
summary_line: openIdConnect · 3 schemes
tags:
- Education
- K-12
- Curriculum
- Learning Management
- Assessment
- EdTech
- Rostering
- Interoperability
- LTI
- OneRoster
- Analytics
---
