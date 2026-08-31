---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Modelop Authentication
name_suffix: Authentication
oauth_flows: []
overview: ModelOp declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: ModelOp
provider_slug: modelop
scheme_count: 3
schemes:
- authorization_server: customer-operated
  description: OAuth 2.0 + OpenID Connect. Applies uniformly across the ModelOp Center web UI, the `moc` CLI, the REST APIs and the Jupyter / RStudio plugins.
  flows_documented:
  - name: C2B (client-to-business)
    note: Interactive end-user login through the enterprise IdP; documented with a PingFederate walkthrough.
  - name: B2B (business-to-business)
    note: Service-to-service token flow between ModelOp Center components and external systems.
  id: oauth2-oidc-bearer
  note: ModelOp explicitly does not bind to one OAuth2 authorization server or IdP implementation; the docs hub carries a per-provider how-to page for each of the five above.
  primary: true
  supported_authorization_servers:
  - PingFederate
  - Amazon Cognito
  - Okta
  - Microsoft Entra ID (formerly Azure Active Directory)
  - Keycloak
  token_formats:
  - JWT
  type: oauth2
- description: SAML 2.0 identity providers are supported indirectly — OAuth2/OIDC fronting a SAML2 IdP — via a separately installed `saml-support-service`.
  docs: https://modelopdocs.atlassian.net/wiki/spaces/MDHV/pages/3159996249/Security+-+SAML+2.0+IdP+Integration
  id: saml2-idp
  primary: false
  type: saml
- deprecated_in: '3.3'
  description: The embedded Camunda WebApp used basic login. From ModelOp Center 3.3, when secured mode with OAuth2/OIDC is enabled, that basic login is replaced by a security filter that admits only ADMIN-group users, and the WebApp is reachable only through the Gateway.
  id: basic-camunda-webapp
  primary: false
  scheme: basic
  type: http
slug: modelop-authentication
source_filename: modelop-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: searched\nsource: >-\n  https://modelopdocs.atlassian.net/wiki/spaces/MDHV/pages/3159996285/ModelOp+Center+Security+-+Oauth2+Integration\n  + .../3159996249/Security+-+SAML+2.0+IdP+Integration\n  + .../3159996790/Supported+OAuth+2.0+Identity+Providers\n  + .../3159996694/Gateway+Authorization+mechanisms\n  + .../3159996726/MLC+Authorization+mechanisms\n  + .../3159996543/Granular+RWX+Details\n  + .../3159992085/Permissions+Administration\nchecked: '2026-08-25'\nderivation_note: >-\n  DERIVED FROM DOCUMENTATION, NOT FROM A SPEC. ModelOp Center is customer-deployed software; its\n  OpenAPI/Swagger document is served only from a customer's own instance\n  (<base>/swagger-ui/webjars/swagger-ui/index.html?urls.primaryName=model-manage), so\n  derive-authentication.py has no openapi/ file to read. Every field below is taken from the\n  public documentation hub.\nsummary: >-\n  ModelOp Center authenticates against the enterprise's own identity provider\
  \ using OAuth 2.0 with\n  OIDC, and authorizes with a group-based read/write/execute (RWX) model backed by AD/LDAP groups.\n  There are no ModelOp-issued API keys and no ModelOp-hosted authorization server — the\n  authorization server is whichever OAuth2 provider the customer already runs.\nschemes:\n  - id: oauth2-oidc-bearer\n    type: oauth2\n    primary: true\n    description: >-\n      OAuth 2.0 + OpenID Connect. Applies uniformly across the ModelOp Center web UI, the `moc`\n      CLI, the REST APIs and the Jupyter / RStudio plugins.\n    token_formats:\n      - JWT\n    flows_documented:\n      - name: C2B (client-to-business)\n        note: Interactive end-user login through the enterprise IdP; documented with a PingFederate walkthrough.\n      - name: B2B (business-to-business)\n        note: Service-to-service token flow between ModelOp Center components and external systems.\n    authorization_server: customer-operated\n    supported_authorization_servers:\n      - PingFederate\n\
  \      - Amazon Cognito\n      - Okta\n      - Microsoft Entra ID (formerly Azure Active Directory)\n      - Keycloak\n    note: >-\n      ModelOp explicitly does not bind to one OAuth2 authorization server or IdP implementation;\n      the docs hub carries a per-provider how-to page for each of the five above.\n  - id: saml2-idp\n    type: saml\n    primary: false\n    description: >-\n      SAML 2.0 identity providers are supported indirectly — OAuth2/OIDC fronting a SAML2 IdP —\n      via a separately installed `saml-support-service`.\n    docs: https://modelopdocs.atlassian.net/wiki/spaces/MDHV/pages/3159996249/Security+-+SAML+2.0+IdP+Integration\n  - id: basic-camunda-webapp\n    type: http\n    scheme: basic\n    primary: false\n    deprecated_in: '3.3'\n    description: >-\n      The embedded Camunda WebApp used basic login. From ModelOp Center 3.3, when secured mode\n      with OAuth2/OIDC is enabled, that basic login is replaced by a security filter that admits\n      only ADMIN-group\
  \ users, and the WebApp is reachable only through the Gateway.\napi_keys:\n  issued: false\n  note: No ModelOp-issued API key, client secret or personal access token scheme is documented.\nauthorization:\n  model: rwx-group-access-control\n  description: >-\n    Read / Write / Execute permissions assigned to enterprise groups per entity, enforced at the\n    lowest levels of every internal ModelOp Center call. Two user categories: Administrators\n    (see all resources, manage Application Forms, Scores Configuration and permissions) and\n    non-administrators (limited to the business units / groups they belong to).\n  group_source: Active Directory / LDAP, surfaced through the OAuth2 OIDC provider\n  multi_tenancy: true\n  enable_flag: |\n    modelop:\n      security:\n        mode: rwx\n  configuration_example: |\n    modelop:\n      security:\n        group-access-rights:\n          default-permissions: read, write, execute\n          collection-permissions:\n            stored-model:\n\
  \              - read\n              - write\n            deployable-model: read, write\n  named_collections:\n    - stored-model      # \"Business Models and Monitors\"\n    - deployable-model  # \"Snapshots\"\n  service_level_authorization:\n    - service: gateway\n      docs: https://modelopdocs.atlassian.net/wiki/spaces/MDHV/pages/3159996694/Gateway+Authorization+mechanisms\n    - service: mlc-service\n      docs: https://modelopdocs.atlassian.net/wiki/spaces/MDHV/pages/3159996726/MLC+Authorization+mechanisms\n      protected_actions:\n        - action: deploy (BPMN deployment)\n          config_key: mlc.camunda.access.rest.deploy.groups\n        - action: signal\n          config_key: mlc.camunda.access.rest.signal.groups\n        - action: signal-responsive\n          config_key: mlc.camunda.access.rest.signal-responsive.groups\n      note: >-\n        Each action is gated on a comma-separated list of group names; admins always pass.\noauth_scopes:\n  published: false\n  note: >-\n\
  \    ModelOp Center does not publish an OAuth SCOPE catalogue. Authorization is expressed as RWX\n    permissions on entity collections held by IdP groups, not as OAuth scope strings, so no\n    scopes/ artifact is emitted and no OAuthScopes pointer is wired. This is the same call made\n    for key-auth providers in this pipeline: authentication/ carries the whole model.\ndata_handling_claim:\n  claim: >-\n    \"ModelOp Center does not store any Customer business data sets; rather, ModelOp Center simply\n    stores references to these data sets to leverage existing SecOps policies for these business\n    data sets.\"\n  source: https://modelopdocs.atlassian.net/wiki/spaces/MDHV/pages/3159996285/ModelOp+Center+Security+-+Oauth2+Integration\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/modelop/refs/heads/main/authentication/modelop-authentication.yml
summary_line: 3 schemes
tags:
- AI Governance
- Model Risk Management
- Machine-Learning
- MLOps
- ModelOps
- AI Lifecycle Automation
- Enterprise Software
- Compliance
- Model Monitoring
- Governance Risk and Compliance
- Artificial Intelligence
---
