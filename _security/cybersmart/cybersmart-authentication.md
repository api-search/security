---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Cybersmart Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: CyberSmart secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: CyberSmart
provider_slug: cybersmart
scheme_count: 1
schemes:
- availability: All CyberSmart Partners regardless of tier; not available to direct customers
  credential_scope: partner-level (covers all managed organisations)
  description: The CyberSmart Ticketing API authenticates with OAuth2 credentials (client ID and client secret) issued at the partner level. A single credential set covers all of a partner's managed organisations. Credentials are retrieved from the CyberSmart partner portal under Settings > CyberSmart API.
  flow: clientCredentials
  name: OAuth2 Partner Credentials
  sources:
  - https://support.cybersmart.co.uk/knowledgebase/s/article/Ticketing-API-Explained
  - https://knowledge.adoptech.co.uk/how-do-i-set-up-my-cybersmart-integration-0
  type: oauth2
slug: cybersmart-authentication
source_filename: cybersmart-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://support.cybersmart.co.uk/knowledgebase/s/article/Ticketing-API-Explained\ndocs: https://support.cybersmart.co.uk/knowledgebase/s/article/Ticketing-API-Explained\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\n  api_key_in: []\nschemes:\n- name: OAuth2 Partner Credentials\n  type: oauth2\n  flow: clientCredentials\n  description: >-\n    The CyberSmart Ticketing API authenticates with OAuth2 credentials (client\n    ID and client secret) issued at the partner level. A single credential set\n    covers all of a partner's managed organisations. Credentials are retrieved\n    from the CyberSmart partner portal under Settings > CyberSmart API.\n  credential_scope: partner-level (covers all managed organisations)\n  availability: All CyberSmart Partners regardless of tier; not available to direct customers\n  sources:\n  - https://support.cybersmart.co.uk/knowledgebase/s/article/Ticketing-API-Explained\n\
  \  - https://knowledge.adoptech.co.uk/how-do-i-set-up-my-cybersmart-integration-0\nnotes: >-\n  No public OpenAPI/Swagger specification is published for the Ticketing API, so\n  this profile is sourced from CyberSmart partner documentation and a partner\n  integration guide rather than derived from a spec. No token or authorization\n  endpoint URLs are documented publicly.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cybersmart/refs/heads/main/authentication/cybersmart-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Cybersecurity
- Compliance
- Cyber Essentials
- Security Certification
- MSP
- Device Security
- GDPR
- SME
---
