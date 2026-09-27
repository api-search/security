---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication for Zenhub GraphQL API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Axiom Zen Authentication
name_suffix: Authentication
oauth_flows: []
overview: ZenHub declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: ZenHub
provider_slug: axiom-zen
scheme_count: 1
schemes:
- evidence: In order to use the GraphQL API, we need to be able to authenticate who is making the request. This is done via a Personal API Key that's associated with your Zenhub account.
  header: Authorization
  how_to_obtain: Generate in the API section of your Zenhub Dashboard; copy the key value when shown.
  location: header
  name: Personal API Key
  type: http-bearer
slug: axiom-zen-authentication
source_filename: axiom-zen-authentication.yml
source_heading: Authentication Profile
source_url: https://support.zenhub.com/article/saml-re-authentication.md
source_yaml: "generated: '2026-09-27'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://support.zenhub.com/article/saml-re-authentication.md\nsources:\n- https://support.zenhub.com/article/saml-re-authentication.md\n- https://support.zenhub.com/article/how-do-i-set-up-my-zenhub-account-and-organization.md\n- https://developers.zenhub.com/graphql-api-docs/getting-started/index.html\ndescription: Authentication for Zenhub GraphQL API\nschemes:\n- type: http-bearer\n  name: Personal API Key\n  evidence: In order to use the GraphQL API, we need to be able to authenticate who is making the request. This is done via a Personal API Key\n    that's associated with your Zenhub account.\n  location: header\n  header: Authorization\n  how_to_obtain: Generate in the API section of your Zenhub Dashboard; copy the key value when shown.\nnote: No OAuth flows, query parameters, or body credentials are documented.\ndocs: https://support.zenhub.com/article/saml-re-authentication.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/axiom-zen/refs/heads/main/authentication/axiom-zen-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Project Management
- GitHub Integration
- AI Automation
- Enterprise
---
