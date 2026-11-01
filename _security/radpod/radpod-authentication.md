---
anonymous_access: false
api_key_in: []
api_specs:
- filename: radpod-openapi-generated.yml
  format: yaml
  label: RadPod API
  slug: radpod-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/radpod/openapi/_ae-authored/radpod-openapi-generated.yml
auth_types: []
description: Compound supports authentication via OpenID Connect (OAuth2 authorization code flow) and SAML 2.0 SSO. SCIM provisioning uses a bearer token sent in an HTTP header.
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Radpod Authentication
name_suffix: Authentication
oauth_flows: []
overview: RadPod declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: RadPod
provider_slug: radpod
scheme_count: 3
schemes:
- authorize_url: https://your-org.okta.com/oauth2/default/v1/authorize
  evidence: This guide walks you through configuring OpenID Connect (OIDC) SSO between Okta and Compound.
  flows:
  - authorization_code
  how_to_obtain: Create an OIDC application in Okta, copy the Client ID, Client Secret, and Issuer URL, and enter them in Compound’s SSO settings.
  name: Okta OIDC
  type: oauth2
- evidence: This guide walks you through configuring SAML 2.0 SSO between Okta and Compound.
  how_to_obtain: Create a SAML application in Okta, upload the IdP metadata XML to Compound, then copy the ACS URL and SP Entity ID from Compound back into Okta.
  name: Okta SAML
  type: other
- evidence: Compound shows a SCIM Endpoint URL and a bearer token (under Copy this token now. It will not be shown again.)
  how_to_obtain: Enable SCIM in Compound to receive a bearer token, then configure Okta SCIM connector to use the token in the Authorization HTTP header.
  name: SCIM Bearer Token
  type: http-bearer
slug: radpod-authentication
source_filename: radpod-authentication.yml
source_heading: Authentication Profile
source_url: https://getcompound.ai/help/getting-started-overview
source_yaml: "generated: '2026-10-22'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://getcompound.ai/help/getting-started-overview\nsources:\n- https://getcompound.ai/help/getting-started-overview\n- https://getcompound.ai/help/okta-oidc-sso-setup\n- https://getcompound.ai/help/okta-saml-sso-setup\n- https://getcompound.ai/help/okta-scim-setup\ndescription: Compound supports authentication via OpenID Connect (OAuth2 authorization code flow) and SAML 2.0 SSO. SCIM provisioning uses a bearer\n  token sent in an HTTP header.\nschemes:\n- type: oauth2\n  name: Okta OIDC\n  evidence: This guide walks you through configuring OpenID Connect (OIDC) SSO between Okta and Compound.\n  flows:\n  - authorization_code\n  authorize_url: https://your-org.okta.com/oauth2/default/v1/authorize\n  how_to_obtain: Create an OIDC application in Okta, copy the Client ID, Client Secret, and Issuer URL, and enter them in Compound’s SSO settings.\n- type: other\n  name: Okta SAML\n\
  \  evidence: This guide walks you through configuring SAML 2.0 SSO between Okta and Compound.\n  how_to_obtain: Create a SAML application in Okta, upload the IdP metadata XML to Compound, then copy the ACS URL and SP Entity ID from Compound\n    back into Okta.\n- type: http-bearer\n  name: SCIM Bearer Token\n  evidence: Compound shows a SCIM Endpoint URL and a bearer token (under Copy this token now. It will not be shown again.)\n  how_to_obtain: Enable SCIM in Compound to receive a bearer token, then configure Okta SCIM connector to use the token in the Authorization HTTP\n    header.\ndocs: https://getcompound.ai/help/getting-started-overview\n"
source_yaml_url: https://artifacts.apis.io/radpod/authentication/radpod-authentication.yml
summary_line: 3 schemes
tags:
- Company
- AI
- Finance
- Platform
- Automation
---
