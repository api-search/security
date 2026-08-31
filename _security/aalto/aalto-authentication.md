---
api_key_in: []
api_specs:
- filename: aalto-facilities-api-openapi.yml
  format: yaml
  label: Aalto Facilities API
  slug: facilities
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aalto/refs/heads/main/openapi/aalto-facilities-api-openapi.yml
- filename: aalto-course-sisu-api-openapi.yml
  format: yaml
  label: Aalto Course API (SISU)
  slug: course-sisu
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aalto/refs/heads/main/openapi/aalto-course-sisu-api-openapi.yml
- filename: aalto-acris-research-api-openapi.yml
  format: yaml
  label: Aalto Research Publications API (Acris gateway)
  slug: acris-research
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aalto/refs/heads/main/openapi/aalto-acris-research-api-openapi.yml
- filename: aalto-projects-costcenters-api-openapi.yml
  format: yaml
  label: Aalto Projects and Cost Centers API
  slug: projects-costcenters
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aalto/refs/heads/main/openapi/aalto-projects-costcenters-api-openapi.yml
- filename: aalto-people-profile-api-openapi.yml
  format: yaml
  label: Aalto People Profile API
  slug: people-profile
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aalto/refs/heads/main/openapi/aalto-people-profile-api-openapi.yml
auth_types: []
description: 'How Aalto University''s institution-operated API surfaces authenticate. Two distinct regimes are in play: every Aalto API Gateway product is API-key gated and returns 403 to an anonymous caller, while the Aaltodoc repository''s OAI-PMH and DSpace REST read surfaces are fully anonymous. Separately, Aalto operates its own Shibboleth SAML 2.0 identity provider for browser-based sign-in to campus services, which is federation infrastructure rather than an API credential.'
kind: authentication
layout: security
method: probed
name: Aalto Authentication
name_suffix: Authentication
oauth_flows: []
overview: Aalto University declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Aalto University
provider_slug: aalto
scheme_count: 0
schemes: []
slug: aalto-authentication
source_filename: aalto-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "---\nname: Aalto University — Authentication\ndescription: >-\n  How Aalto University's institution-operated API surfaces authenticate. Two distinct regimes are in\n  play: every Aalto API Gateway product is API-key gated and returns 403 to an anonymous caller, while\n  the Aaltodoc repository's OAI-PMH and DSpace REST read surfaces are fully anonymous. Separately,\n  Aalto operates its own Shibboleth SAML 2.0 identity provider for browser-based sign-in to campus\n  services, which is federation infrastructure rather than an API credential.\ngenerated: '2026-08-30'\nmethod: probed\nsource: >-\n  securitySchemes read from Aalto's own OpenAPI documents on\n  https://3scale.apps.ocp4.aalto.fi/api_docs/services.json, plus live unauthenticated probes of each\n  declared server on 2026-08-30.\nx-operator: institution\nurl: https://raw.githubusercontent.com/api-evangelist/aalto/main/authentication/aalto-authentication.yml\n\nmechanisms:\n  - id: gateway-api-key-header\n    type: apiKey\n\
  \    label: Aalto API Gateway — API key in header\n    in: header\n    parameter_names:\n      - X-ApiKey\n      - USER-KEY\n    applies_to:\n      - Aalto project and costcenter API (X-ApiKey)\n      - Acris Research Publications API (USER-KEY)\n    onboarding: >-\n      Register an application on the Aalto API Gateway developer portal at\n      https://3scale.apps.ocp4.aalto.fi/ (front door https://apiportal.aalto.fi/) and a key is issued\n      per application. Registration requires an Aalto account; the portal advertises \"Register\",\n      \"Get Your API Key\" and \"Create Your App\" as the three onboarding steps.\n    method: searched\n    source: https://3scale.apps.ocp4.aalto.fi/api_docs/services/13.json\n\n  - id: gateway-api-key-query\n    type: apiKey\n    label: Aalto API Gateway — API key in query string\n    in: query\n    parameter_names:\n      - USER_KEY\n    applies_to:\n      - Sisu Course API\n    method: searched\n    source: https://3scale.apps.ocp4.aalto.fi/api_docs/services/27.json\n\
  \n  - id: gateway-undeclared\n    type: apiKey\n    label: Gateway-enforced key, not declared in the contract\n    in: unknown\n    applies_to:\n      - Aalto facilities api\n      - Aalto people profile api\n    note: >-\n      Neither document declares a securityScheme, but both declared servers reject an anonymous call\n      at the 3scale edge. The enforcement is real and the contract does not describe it — a genuine\n      contract gap, recorded here rather than invented into the spec.\n    method: probed\n    source: https://facilities.api.aalto.fi/api/aalto/facilities/v1/buildings\n\n  - id: anonymous-read\n    type: none\n    label: Anonymous public read\n    applies_to:\n      - Aaltodoc OAI-PMH 2.0 (https://aaltodoc.aalto.fi/server/oai/request)\n      - Aaltodoc DSpace 9.2 REST API (https://aaltodoc.aalto.fi/server/api)\n      - Linked Open Aalto Data SPARQL (http://ldf.fi/loa/sparql, POST only)\n    note: >-\n      These are the only Aalto surfaces that answer a credential-free\
  \ request with data. Everything on\n      the API Gateway does not.\n    method: probed\n    source: https://aaltodoc.aalto.fi/server/oai/request?verb=Identify\n\n  - id: shibboleth-saml\n    type: saml\n    label: Shibboleth SAML 2.0 identity provider (browser SSO, not an API credential)\n    entity_id: https://idp.aalto.fi/idp/shibboleth\n    scope: aalto.fi\n    federation: Haka (Finnish higher-education federation), onward to eduGAIN\n    method: probed\n    source: https://idp.aalto.fi/idp/shibboleth\n\nanonymous_probe_results:\n  - url: https://facilities.api.aalto.fi/api/aalto/facilities/v1/buildings\n    status: 403\n    body: Authentication parameters missing\n  - url: https://course.api.aalto.fi/api/sisu/v1/courseunits\n    status: 403\n  - url: https://research.api.aalto.fi/api/acris/v1/research-outputs\n    status: 403\n  - url: https://aaltopeople.api.aalto.fi/api/aaltopeople/v1/profiles\n    status: 403\n  - url: https://api.aalto.fi/api/dw_projects/schools\n    status: 403\n\
  \  - url: https://aaltodoc.aalto.fi/server/oai/request?verb=Identify\n    status: 200\n  - url: https://aaltodoc.aalto.fi/server/api\n    status: 200\n\noauth: false\nscopes: none_declared\nnotes: >-\n  No OAuth 2.0 authorization server, no declared scopes, and no machine-readable onboarding document\n  were found on any Aalto surface. The gateway's key issuance is a human web flow behind an Aalto\n  account, so third-party access to the five gateway products is not self-service for the public.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aalto/refs/heads/main/authentication/aalto-authentication.yml
summary_line: 0 schemes
tags:
- University
- Higher Education
- Education
- Finland
- Europe
- Public Research University
- Research
- Research Data
- Open Data
- Linked Data
- Course Catalog
- Identity Federation
- Research Computing
- Library
- API Gateway
---
