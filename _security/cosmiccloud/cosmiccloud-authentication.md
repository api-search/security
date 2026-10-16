---
anonymous_access: false
api_key_in: []
auth_types: []
description: Cosmiccloud supports authentication via JWTs using a JWKS URI or via Access Key Secrets.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Cosmiccloud Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cosmiccloud declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Cosmiccloud
provider_slug: cosmiccloud
scheme_count: 2
schemes:
- evidence: With Cosmocloud, you can integrate with any and every JWT Based Authentication provider by simply adding your JWKS URI
  how_to_obtain: Generate your JWKS URI on the SSO provider and add it in the auth secret.
  name: JWT
  type: http-bearer
- evidence: Auth Type - Access Key Secret
  how_to_obtain: Generate your access keys on the SSO provider and add them in the auth secret.
  name: Access Key Secret
  type: apiKey
slug: cosmiccloud-authentication
source_filename: cosmiccloud-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.cosmocloud.io/advanced-guide/configuring-authentication.md
source_yaml: "generated: '2026-10-11'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.cosmocloud.io/advanced-guide/configuring-authentication.md\nsources:\n- https://docs.cosmocloud.io/advanced-guide/configuring-authentication.md\n- https://docs.cosmocloud.io/advanced-guide/configuring-authentication/sso-providers.md\n- https://docs.cosmocloud.io/advanced-guide/configuring-authentication/sso-providers/aws-cognito.md\n- https://docs.cosmocloud.io/advanced-guide/configuring-authentication/authentication-concepts.md\ndescription: Cosmiccloud supports authentication via JWTs using a JWKS URI or via Access Key Secrets.\nschemes:\n- type: http-bearer\n  name: JWT\n  evidence: With Cosmocloud, you can integrate with any and every JWT Based Authentication provider by simply adding your JWKS URI\n  how_to_obtain: Generate your JWKS URI on the SSO provider and add it in the auth secret.\n- type: apiKey\n  name: Access Key Secret\n  evidence: Auth Type - Access\
  \ Key Secret\n  how_to_obtain: Generate your access keys on the SSO provider and add them in the auth secret.\ndocs: https://docs.cosmocloud.io/advanced-guide/configuring-authentication.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cosmiccloud/refs/heads/main/authentication/cosmiccloud-authentication.yml
summary_line: 2 schemes
tags:
- Cloud
- DevOps
- Automation
- Deployment
- Startup
- Company
---
