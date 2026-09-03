---
api_key_in: []
auth_types: []
description: 'How the machine-readable surfaces the American University of Beirut operates authenticate. Three regimes are in play and they behave very differently. The AUB ScholarWorks repository read surfaces — DSpace REST and OAI-PMH — are fully anonymous: no key, no account, no rate-limit gate was encountered. The AUB-hosted Moodle Web Services API is token-gated and issues tokens only to AUB accounts. And AUB operates its own Shibboleth SAML 2.0 identity provider, which is browser-based federated sign-in infrastructure rather than an API credential, plus an LTI 1.3 OAuth 2.0 client-credentials token endpoint for external learning tools. AUB publishes no developer portal, issues no public API keys and documents no self-service credential path of any kind.'
kind: authentication
layout: security
method: probed
name: Aub Authentication
name_suffix: Authentication
oauth_flows: []
overview: American University of Beirut declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: American University of Beirut
provider_slug: aub
scheme_count: 0
schemes: []
slug: aub-authentication
source_filename: aub-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "---\nname: American University of Beirut — Authentication\ndescription: >-\n  How the machine-readable surfaces the American University of Beirut operates authenticate. Three\n  regimes are in play and they behave very differently. The AUB ScholarWorks repository read surfaces\n  — DSpace REST and OAI-PMH — are fully anonymous: no key, no account, no rate-limit gate was\n  encountered. The AUB-hosted Moodle Web Services API is token-gated and issues tokens only to AUB\n  accounts. And AUB operates its own Shibboleth SAML 2.0 identity provider, which is browser-based\n  federated sign-in infrastructure rather than an API credential, plus an LTI 1.3 OAuth 2.0\n  client-credentials token endpoint for external learning tools. AUB publishes no developer portal,\n  issues no public API keys and documents no self-service credential path of any kind.\ngenerated: '2026-09-01'\nmethod: probed\nsource: >-\n  Live unauthenticated probes of scholarworks.aub.edu.lb, lms.aub.edu.lb and idp.aub.edu.lb\
  \ on\n  2026-09-01. No securityScheme was read from any contract, because AUB publishes none.\nx-operator: institution\nurl: https://raw.githubusercontent.com/api-evangelist/aub/main/authentication/aub-authentication.yml\n\nmechanisms:\n  - id: scholarworks-anonymous-read\n    type: none\n    label: AUB ScholarWorks — anonymous read\n    applies_to:\n      - AUB ScholarWorks DSpace REST API\n      - AUB ScholarWorks OAI-PMH\n    detail: >-\n      /server/api/authn/status returns okay true, authenticated false, authenticationMethod null to\n      an anonymous caller, and the discovery, community, collection and item endpoints return data\n      without credentials — 25 communities and 24,318 items were enumerated anonymously. OAI-PMH is\n      equally open. Write and workflow endpoints exist in the DSpace link index but are not reachable\n      anonymously.\n    method: probed\n    source: https://scholarworks.aub.edu.lb/server/api/authn/status\n\n  - id: scholarworks-shibboleth-login\n\
  \    type: saml\n    label: AUB ScholarWorks — Shibboleth SSO for authenticated actions\n    applies_to:\n      - AUB ScholarWorks DSpace REST API\n    detail: >-\n      DSpace's Shibboleth authentication method is enabled: /server/api/authn/shibboleth returns a\n      302 back into the repository, delegating identity to AUB's institutional IdP. Submission and\n      workflow actions therefore require an AUB account through SAML, not an API key.\n      POST /server/api/authn/login returns 403 with application/json to an unauthenticated caller.\n    method: probed\n    source: https://scholarworks.aub.edu.lb/server/api/authn/shibboleth\n\n  - id: moodle-webservice-token\n    type: apiKey\n    label: Moodle Web Services — wstoken\n    in: query\n    parameter_names:\n      - wstoken\n    applies_to:\n      - AUB Moodle Web Services (REST)\n    detail: >-\n      An anonymous call returns an XML fault with ERRORCODE invalidtoken and MESSAGE \"Invalid token -\n      token not found\", which\
  \ confirms the service is enabled and token-gated. Moodle tokens are\n      issued per user and per external service from within the LMS; there is no public registration\n      path and no documented self-service issuance for outside developers.\n    onboarding: >-\n      AUB account required. Tokens are provisioned inside lms.aub.edu.lb by an administrator or via\n      the user's own security-keys page; requests are routed through the AUB IT service desk.\n    method: probed\n    source: https://lms.aub.edu.lb/webservice/rest/server.php\n\n  - id: lti-client-credentials\n    type: oauth2\n    label: LTI 1.3 Advantage — OAuth 2.0 client credentials with signed JWT\n    applies_to:\n      - AUB Moodle LTI 1.3 platform endpoints\n    detail: >-\n      /mod/lti/token.php is the LTI Advantage service token endpoint and returns\n      {\"error\":\"invalid_request\"} with HTTP 400 to an empty POST — a conformant OAuth 2.0 error, not\n      a 404. The matching public JWKS at /mod/lti/certs.php\
  \ is served anonymously and carries a live\n      RS256 key. Credentials are established through an LTI 1.3 tool registration performed by AUB,\n      not issued on request.\n    method: probed\n    source: https://lms.aub.edu.lb/mod/lti/token.php\n\n  - id: shibboleth-idp\n    type: saml\n    label: AUB Shibboleth Identity Provider — institutional SSO\n    applies_to:\n      - AUB Shibboleth Identity Provider (SAML 2.0)\n      - InCommon federation registration (AUB IdP)\n    detail: >-\n      entityID https://idp.aub.edu.lb/idp/shibboleth, scope aub.edu.lb, four SingleSignOnService\n      bindings (Shibboleth SSO, SAML2 POST, SAML2 Redirect, SAML2 POST-SimpleSign), separate\n      back-channel and front-channel signing certificates. Registered in InCommon with the REFEDS\n      Sirtfi entity category asserted. This is browser-mediated federated authentication for humans;\n      it is not a machine credential and cannot be used to call an API directly.\n    method: probed\n    source:\
  \ https://idp.aub.edu.lb/idp/shibboleth\n\nnotes:\n  - >-\n    No API key, OAuth client registration, or developer account can be obtained from AUB by an\n    outside party. Every gated surface here is gated on holding an AUB identity, which makes the\n    anonymous repository read surfaces the entire public API footprint of the institution.\n  - >-\n    api.aub.edu.lb returns HTTP 403 from IIS with no WWW-Authenticate header and no service behind\n    it. It is not an authentication gate; it is an unused hostname.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aub/refs/heads/main/authentication/aub-authentication.yml
summary_line: 0 schemes
tags:
- University
- Higher Education
- Education
- Lebanon
- Middle East
- Private Research University
- Research
- Research Data
- Open Access
- Libraries
- Institutional Repository
- Identity Federation
- Learning Management
---
