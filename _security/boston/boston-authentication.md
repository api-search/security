---
api_key_in: []
api_specs:
- filename: boston-wordpress-api-openapi.yml
  format: yaml
  label: Boston University WordPress REST API
  slug: wordpress-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boston/refs/heads/main/openapi/boston-wordpress-api-openapi.yml
auth_types: []
description: How access is controlled on the surfaces Boston University itself operates. No credentials of any kind were used; every observation below comes from an anonymous HTTP GET.
kind: authentication
layout: security
method: probed
name: Boston Authentication
name_suffix: Authentication
oauth_flows: []
overview: Boston University declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Boston University
provider_slug: boston
scheme_count: 0
schemes: []
slug: boston-authentication
source_filename: boston-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "# x-method: derived\n# x-source-url: https://www.bu.edu/wp-json/\n# Authorship: written by API Evangelist from live, unauthenticated probes on 2026-08-30.\n# The structured `method: probed` below is the university pipeline's evidence class for\n# the same fact; `x-method` is the authorship class provenance.yml records.\nspecification: API Evangelist Authentication\nspecificationVersion: '0.1'\nprovider: Boston University\nproviderId: boston\ngenerated: '2026-08-30'\nmethod: probed\nsource: unauthenticated live probes of https://www.bu.edu/wp-json/ on 2026-08-30\ndescription: >-\n  How access is controlled on the surfaces Boston University itself operates. No credentials of any\n  kind were used; every observation below comes from an anonymous HTTP GET.\nsurfaces:\n  - name: Boston University WordPress REST API\n    x-operator: institution\n    baseURL: https://www.bu.edu/wp-json\n    scheme: none-for-reads / cookie+nonce-for-privileged\n    description: >-\n      WordPress\
  \ core authentication. Anonymous callers get the public read surface. Privileged\n      routes reject anonymous callers with HTTP 401 and the WordPress `rest_forbidden` code. Boston\n      University publishes no API keys, no OAuth flow, and no developer registration for this\n      interface — it is the CMS's own REST layer, incidentally public, not a productized API.\n    observed:\n      public:\n        - path: /\n          status: 200\n          note: Full route discovery document, 237 routes, 15 namespaces.\n        - path: /bu-alert/v1\n          status: 200\n          note: Namespace discovery document.\n        - path: /bu-navigation/v1\n          status: 200\n        - path: /bu-blocks/v1/collection\n          status: 200\n        - path: /bu-blocks/v1/search\n          status: 200\n        - path: /bu-prepress/v1/event\n          status: 200\n        - path: /wp/v2/pages\n          status: 200\n        - path: /wp/v2/types\n          status: 200\n        - path: /wp/v2/taxonomies\n\
  \          status: 200\n      gated:\n        - path: /bu-navigation/v1/parents\n          status: 401\n          code: rest_forbidden\n        - path: /bu-slideshow/v1/shows\n          status: 401\n          code: rest_forbidden\n        - path: /bu-access-control/v1/get-groups\n          status: 401\n          code: rest_forbidden\n    observations:\n      - severity: informational\n        description: >-\n          GET /bu-blocks/v1/search returns objects carrying \"status\":\"draft\" to an unauthenticated\n          caller — unpublished editorial content is reachable through this route without\n          credentials. Recorded as an access-clarity observation from a public probe. No draft\n          content is reproduced in this repository's examples.\n        observed: '2026-08-30'\n  - name: OpenBU repository (DSpace 7.6 / OAI-PMH)\n    x-operator: tenant\n    baseURL: https://open.bu.edu/server\n    scheme: none\n    description: >-\n      Both the OAI-PMH endpoint and the DSpace\
  \ 7 REST API answer anonymous callers. Write and\n      submission workflows are behind DSpace authn at /server/api/authn. Operated for Boston\n      University by Atmire.\n    observed:\n      public:\n        - path: /oai/request?verb=Identify\n          status: 200\n        - path: /api\n          status: 200\n        - path: /api/core/communities\n          status: 200\n  - name: AI API Access (Azure OpenAI / Amazon Bedrock)\n    x-operator: tenant\n    scheme: request-form\n    description: >-\n      Boston University IS&T brokers LLM API keys to affiliated faculty, researchers, staff and\n      departments. Access requires financial-administrator approval and an AI API Key Request Form;\n      provisioning details and documentation are supplied only after approval. The underlying APIs\n      are Microsoft's and Amazon's, not Boston University's — BU operates the key-issuing process,\n      which is not itself a machine-readable interface.\n    observed:\n      documentation:\n  \
  \      - url: https://www.bu.edu/tech/services/cccs/collaboration/conversational-ai/ai-api-access/\n          status: 200\n  - name: Boston University Shibboleth Identity Provider\n    x-operator: institution\n    baseURL: https://shib.bu.edu/idp\n    scheme: saml2-sso\n    description: >-\n      SAML 2.0 single sign-on for the bu.edu and alum.bu.edu scopes. The entity metadata is public\n      and anonymous; the SSO endpoints themselves are only meaningful inside a SAML flow.\n    observed:\n      public:\n        - path: /shibboleth\n          status: 200\n          note: SAML 2.0 EntityDescriptor.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/boston/refs/heads/main/authentication/boston-authentication.yml
summary_line: 0 schemes
tags:
- University
- Higher Education
- Education
- United States
- Massachusetts
- Private Research University
- Research
- Research Data
- Library
- Identity Federation
- Content Management
- Open Access
---
