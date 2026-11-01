---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication schemes for Singpass as described in the provided pages.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Singpass Authentication
name_suffix: Authentication
oauth_flows: []
overview: Singpass declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Singpass
provider_slug: singpass
scheme_count: 1
schemes:
- evidence: To initiate the CIBA flow, RPs must authenticate itself with Singpass using client assertion JWT.
  how_to_obtain: RP creates a JWT assertion and includes it in the client_assertion form parameter when calling the backchannel authentication endpoint.
  location: body
  name: client_assertion JWT
  scopes:
  - openid
  type: oauth2
slug: singpass-authentication
source_filename: singpass-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.developer.singpass.gov.sg/docs/singpass-developer-portal-sdp/understanding-the-app-config-fields/token-based-authentication.md
source_yaml: "generated: '2026-10-27'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.developer.singpass.gov.sg/docs/singpass-developer-portal-sdp/understanding-the-app-config-fields/token-based-authentication.md\nsources:\n- https://docs.developer.singpass.gov.sg/docs/singpass-developer-portal-sdp/understanding-the-app-config-fields/token-based-authentication.md\n- https://docs.developer.singpass.gov.sg/docs/singpass-developer-docs/client-initiated-backchannel-authentication-ciba/quick-start.md\n- https://docs.developer.singpass.gov.sg/docs/singpass-developer-docs/client-initiated-backchannel-authentication-ciba/step-up-authentication-using-push-notifications.md\n- https://docs.developer.singpass.gov.sg/docs/singpass-developer-docs/client-initiated-backchannel-authentication-ciba/step-up-authentication-using-push-notifications/backchannel-authentication-endpoint.md\ndescription: Authentication schemes for Singpass as described in the provided pages.\n\
  schemes:\n- type: oauth2\n  name: client_assertion JWT\n  evidence: To initiate the CIBA flow, RPs must authenticate itself with Singpass using client assertion JWT.\n  location: body\n  scopes:\n  - openid\n  how_to_obtain: RP creates a JWT assertion and includes it in the client_assertion form parameter when calling the backchannel authentication\n    endpoint.\ndocs: https://docs.developer.singpass.gov.sg/docs/singpass-developer-portal-sdp/understanding-the-app-config-fields/token-based-authentication.md\n"
source_yaml_url: https://artifacts.apis.io/singpass/authentication/singpass-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Identity
- Authentication
- Government
- Singapore
---
