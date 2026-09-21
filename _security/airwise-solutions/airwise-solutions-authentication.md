---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: probed
name: Airwise Solutions Authentication
name_suffix: Authentication
oauth_flows: []
overview: AirWise Solutions declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: AirWise Solutions
provider_slug: airwise-solutions
scheme_count: 1
schemes:
- authorization_endpoint: https://sso.airwisesolutions.app/oauth2/authorize
  name: airwise-sso
  openIdConnectUrl: https://cognito-idp.us-west-2.amazonaws.com/us-west-2_5xk7sQaJU/.well-known/openid-configuration
  provider: Amazon Cognito
  response_types_supported:
  - code
  - token
  scopes_supported:
  - openid
  - email
  - phone
  - profile
  token_endpoint: https://sso.airwisesolutions.app/oauth2/token
  type: openIdConnect
slug: airwise-solutions-authentication
source_filename: airwise-solutions-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-20'\nmethod: probed\nsource: https://cognito-idp.us-west-2.amazonaws.com/us-west-2_5xk7sQaJU/.well-known/openid-configuration\ndocs: https://developer.airwisesolutions.app/\nschemes:\n- name: airwise-sso\n  type: openIdConnect\n  openIdConnectUrl: https://cognito-idp.us-west-2.amazonaws.com/us-west-2_5xk7sQaJU/.well-known/openid-configuration\n  provider: Amazon Cognito\n  authorization_endpoint: https://sso.airwisesolutions.app/oauth2/authorize\n  token_endpoint: https://sso.airwisesolutions.app/oauth2/token\n  scopes_supported:\n  - openid\n  - email\n  - phone\n  - profile\n  response_types_supported:\n  - code\n  - token\nnote: This is the platform identity provider used by the AirWise web apps and the developer portal sign-in. Which schemes individual API routes require is documented only behind the developer-portal sign-in\n  and is not recorded here.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airwise-solutions/refs/heads/main/authentication/airwise-solutions-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Drones
- UAS
- Aviation
- Airspace
- UTM
- Public Safety
- Critical Infrastructure
- Geospatial
---
