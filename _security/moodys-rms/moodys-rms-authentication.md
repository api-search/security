---
api_key_in:
- header
api_specs:
- filename: overview
  format: yaml
  label: Moody's RMS Platform APIs
  slug: platform-apis
  spec_type: Postman
  url: https://www.postman.com/rms-developers/rms-developers/overview
- filename: moodys-rms-risk-modeler-openapi.yml
  format: yaml
  label: Moody's RMS Risk Modeler API
  slug: risk-modeler-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moodys-rms/refs/heads/main/openapi/moodys-rms-risk-modeler-openapi.yml
- filename: moodys-rms-data-bridge-openapi.json
  format: json
  label: Moody's RMS Data Bridge API
  slug: data-bridge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moodys-rms/refs/heads/main/openapi/moodys-rms-data-bridge-openapi.json
- filename: moodys-rms-location-intelligence-openapi.yaml
  format: yaml
  label: Moody's RMS Location Intelligence API
  slug: location-intelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moodys-rms/refs/heads/main/openapi/moodys-rms-location-intelligence-openapi.yaml
- filename: 21620294-578a748b-78a6-4a3a-b4b3-5c5380b7848e
  format: yaml
  label: Moody's RMS Climate On Demand API
  slug: climate-on-demand-api
  spec_type: Postman
  url: https://www.postman.com/rms-developers/workspace/cod/collection/21620294-578a748b-78a6-4a3a-b4b3-5c5380b7848e
auth_types:
- apiKey
- accessToken
description: ''
kind: authentication
layout: security
method: searched
name: Moodys Rms Authentication
name_suffix: Authentication
oauth_flows: []
overview: Moody's RMS secures its APIs with apiKey and accessToken across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Moody's RMS
provider_slug: moodys-rms
scheme_count: 1
schemes:
- description: An API key is a token that enables a client application to make requests to tenant applications running on Intelligent Risk Platform.
  in: header
  name: RMS_Auth
  parameter: Authorization
  sources:
  - openapi/moodys-rms-data-bridge-openapi.json
  - openapi/moodys-rms-location-intelligence-openapi.yaml
  - openapi/moodys-rms-risk-modeler-openapi.yml
  type: apiKey
slug: moodys-rms-authentication
source_filename: moodys-rms-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: openapi/moodys-rms-data-bridge-openapi.json, openapi/moodys-rms-location-intelligence-openapi.yaml,\n  openapi/moodys-rms-risk-modeler-openapi.yml\ndocs: https://developer.rms.com/platform/docs/authentication-and-authorization\nsummary:\n  types:\n  - apiKey\n  - accessToken\n  api_key_in:\n  - header\n  self_serve: false\n  recommended: apiKey\nschemes:\n- name: RMS_Auth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: An API key is a token that enables a client application to make requests to tenant\n    applications running on Intelligent Risk Platform.\n  sources:\n  - openapi/moodys-rms-data-bridge-openapi.json\n  - openapi/moodys-rms-location-intelligence-openapi.yaml\n  - openapi/moodys-rms-risk-modeler-openapi.yml\nmethods:\n- method: api-key\n  header: Authorization\n  prefix: none\n  lifetime: long-lived\n  bound_to: A project or client application, not a user account.\n  issuance: >-\n  \
  \  Created and managed by tenant administrators in Admin Center. Developers must contact their tenant\n    administrator to acquire an API key. There is no self-serve signup, free tier or sandbox.\n  recommended_for: production\n  example: |-\n    curl --location --request GET 'https://{host}/riskmodelerv1/datasources' \\\n      --header 'Authorization: {api_key}'\n  admin_docs: https://support.rms.com/o/html-doc/OLH_ContentRLRB_Online_Library/Content/IRP_Admin/GeneratingAPIKeys.htm\n- method: access-token\n  header: Authorization\n  style: bearer\n  lifetime: session\n  bound_to: A user account, accessed on that user's behalf.\n  recommended_for: evaluation and testing\n  note: >-\n    The provider explicitly recommends API keys over tokens for production because keys are long-lived\n    and require no refresh. No authorization endpoint, token endpoint, flow or scope list is published,\n    so this is not a discoverable OAuth 2.0 profile — hence no scopes/ artifact.\nauthorization:\n\
  \  model: role-based access control with group-based access rights\n  description: >-\n    The API key or access token encodes the access rights and permissions granted to the client. A key is\n    mapped to one or more groups and inherits the roles assigned to those groups. Entitlements gate which\n    products (Risk Modeler, UnderwriteIQ, ExposureIQ, TreatyIQ) the caller can reach.\n  notable_roles:\n  - name: IRP Agentic Tools User\n    grants:\n    - {action: Access Platform MCP Server, level: read}\n    - {action: Execute APIs with Platform MCP Server, level: write}\n    note: Required for any MCP client connecting to the Platform MCP Server.\n  docs: https://developer.rms.com/platform/docs/access-control\noauth2: false\nopenid_connect: false\nmutual_tls: false\nscopes_published: false\ndiscovery:\n  openid_configuration: not-served\n  oauth_authorization_server: not-served\n  note: See well-known/moodys-rms-well-known.yml for the full probe record.\nhosts:\n- https://api-use1.rms.com\n\
  - https://api-euw1.rms.com\ntransport_security: >-\n  All calls to and from the Intelligent Risk Platform are encrypted. TLS 1.3 was negotiated on\n  api-use1.rms.com and developer.rms.com on 2026-07-25.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moodys-rms/refs/heads/main/authentication/moodys-rms-authentication.yml
summary_line: apiKey/accessToken · 1 scheme
tags:
- Insurance
- United States
- Property and Casualty
- Reinsurance
- Risk Data
- Catastrophe Modeling
- Underwriting
- Climate Risk
- Geocoding
- Analytics
---
