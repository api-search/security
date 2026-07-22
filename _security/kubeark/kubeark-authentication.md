---
api_key_in:
- workflow node input (vault-backed)
auth_types:
- openIdConnect
- oauth2
- saml2
- ldap
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Kubeark Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kubeark secures its APIs with openIdConnect, oauth2, saml2, ldap, and apiKey across 0 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Kubeark
provider_slug: kubeark
scheme_count: 0
schemes: []
slug: kubeark-authentication
source_filename: kubeark-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.kubeark.com/kubeark-identity\ndocs: https://docs.kubeark.com/kubeark-identity\nnote: >-\n  DERIVED-FROM-SPEC WAS NOT POSSIBLE: Kubeark publishes no OpenAPI/Swagger and exposes no\n  public API host, so there are no securitySchemes to aggregate. This profile is searched\n  from the documentation instead. Two distinct auth surfaces exist and are recorded\n  separately: (1) how humans/IdPs authenticate INTO the Kubeark platform, and (2) how\n  workflow nodes authenticate OUT to target systems.\nsummary:\n  types:\n  - openIdConnect\n  - oauth2\n  - saml2\n  - ldap\n  - apiKey\n  api_key_in:\n  - workflow node input (vault-backed)\n  oauth2_flows: []\n  oauth2_flows_note: >-\n    The docs name OAuth2/OIDC support but publish no flow names, authorization URL or\n    token URL, so no flow list is asserted here.\nplatform_authentication:\n  component: Kubeark Identity\n  description: >-\n    Kubeark Identity is the platform's\
  \ bundled identity provider. It manages digital\n    identities, authenticates users, and brokers access to applications. It signs JSON Web\n    Tokens for OAuth and OIDC, and generates a self-signed certificate on first start\n    (valid 1 year, rotatable, also usable for SAML providers/sources).\n  protocols:\n  - id: saml2\n    name: SAML2\n  - id: ldap\n    name: LDAP\n  - id: oauth2\n    name: OAuth2\n  - id: oidc\n    name: OpenID Connect\n  - id: oauth1\n    name: OAuth1\n    note: listed under federation protocols\n  - id: scim\n    name: SCIM\n    note: listed as a supported provider protocol for identity provisioning\n  federation:\n    sso: true\n    docs: https://docs.kubeark.com/federation-and-single-sign-on-sso\n    description: >-\n      Federation and Single Sign On lets users authenticate against an external identity\n      provider of their choice and authorize access to applications and services.\n  session:\n    revoke_previous_sessions: >-\n      Optional setting revokes\
  \ a user's previous sessions on login; documented as having\n      no effect on OAuth refresh tokens.\n  auth_method_context: >-\n    An auth_method property is set by the Password stage, the Authenticator validation\n    stage, the OAuth2 Provider, and by API authentication, depending on which method was\n    used.\nworkflow_authentication:\n  description: >-\n    Workflow nodes authenticate to external and Kubernetes targets using credentials\n    supplied as node inputs and stored in a vault rather than inline.\n  mechanisms:\n  - id: api-token\n    name: Api Token\n    description: >-\n      Node input field carrying the token used to authenticate an action, e.g. the token\n      used to add a Kubeark cluster, or the token kubectl uses against the Kubernetes\n      cluster API.\n    used_by:\n    - Add Kubeark Cluster action\n    - kubectl action\n    - deployment actions\n  - id: kubeconfig\n    name: Kubeconfig\n    description: >-\n      Uploaded file or inline text containing cluster\
  \ server addresses, user credentials\n      and context, used by Kubeark to interact with a Kubernetes cluster.\n  - id: oauth-provider-token\n    name: OAuth provider token\n    description: >-\n      Since the October 2024 release, workflows can retrieve tokens through mainstream\n      OAuth identity providers (GitHub, Salesforce, Google, Microsoft and others) for use\n      when interacting with forms embedded in workflows.\n  credential_storage:\n  - id: local-vault\n    name: Local Vault\n    docs: https://docs.kubeark.com/local-vault\n    scope: workspace\n  - id: global-vault\n    name: Global Vault\n    docs: https://docs.kubeark.com/global-vault\n    scope: platform\n  vault_description: >-\n    Vaults securely store and provide access to secrets such as passwords and API tokens\n    so credentials are referenced by nodes rather than embedded in workflow definitions.\nauthorization:\n  model: Roles and Permissions\n  docs: https://docs.kubeark.com/roles-and-permissions\n  scopes_published:\
  \ false\n  scopes_note: >-\n    No OAuth scope reference or permission-string registry is published, so no scopes/\n    artifact is asserted for this provider.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kubeark/refs/heads/main/authentication/kubeark-authentication.yml
summary_line: openIdConnect/oauth2/saml2/ldap/apiKey · 0 schemes
tags:
- Company
- Orchestration
- Automation
- Workflow Automation
- Integration
- Kubernetes
- Infrastructure as Code
- Terraform
- Identity and Access Management
- Agentic AI
- DevOps
- Self-Hosted
---
