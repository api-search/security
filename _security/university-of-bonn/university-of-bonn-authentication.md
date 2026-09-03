---
api_key_in: []
api_specs:
- filename: university-of-bonn-datasets-api-openapi.yml
  format: yaml
  label: University of Bonn Datasets API
  slug: university-of-bonn-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-bonn/refs/heads/main/openapi/university-of-bonn-datasets-api-openapi.yml
- filename: university-of-bonn-info-api-openapi.yml
  format: yaml
  label: University of Bonn Info API
  slug: university-of-bonn-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-bonn/refs/heads/main/openapi/university-of-bonn-info-api-openapi.yml
- filename: university-of-bonn-metrics-api-openapi.yml
  format: yaml
  label: University of Bonn Metrics API
  slug: university-of-bonn-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-bonn/refs/heads/main/openapi/university-of-bonn-metrics-api-openapi.yml
- filename: university-of-bonn-search-api-openapi.yml
  format: yaml
  label: University of Bonn Search API
  slug: university-of-bonn-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-bonn/refs/heads/main/openapi/university-of-bonn-search-api-openapi.yml
auth_types:
- none
- saml2
- api_key
description: 'The University of Bonn operates its own authentication estate and publishes no public API authorization server. Its one genuinely public API surface — the bonndata Dataverse read subset and the two OAI-PMH endpoints — requires no credentials at all; everything credentialed terminates at the institution''s Shibboleth Identity Provider or at a per-account token issued by an institutional service. There is no developer self-service path: an unaffiliated developer cannot obtain a token for any Bonn system.'
kind: authentication
layout: security
method: probed
name: University Of Bonn Authentication
name_suffix: Authentication
oauth_flows: []
overview: University of Bonn secures its APIs with none, saml2, and api_key across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: University of Bonn
provider_slug: university-of-bonn
scheme_count: 4
schemes:
- applies_to:
  - https://bonndata.uni-bonn.de/api/search
  - https://bonndata.uni-bonn.de/api/datasets
  - https://bonndata.uni-bonn.de/api/info/version
  - https://bonndata.uni-bonn.de/api/info/metrics/datasets
  - https://bonndata.uni-bonn.de/oai
  - https://bonndoc.ulb.uni-bonn.de/oai/request
  - https://gitlab.uni-bonn.de/api/v4/projects
  evidence: All of the above returned 200 with real payloads to anonymous, un-credentialed requests on 2026-09-01. The bonndata OpenAPI documents in this repo cover exactly this keyless subset and nothing else.
  name: No authentication (public read)
  type: none
  x-operator: institution
- bindings:
  - urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect
  - urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST
  - urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST-SimpleSign
  endpoints:
    artifact_resolution: https://shibboleth.uni-bonn.de:8443/idp/profile/SAML2/SOAP/ArtifactResolution
    slo: https://shibboleth.uni-bonn.de/idp/profile/SAML2/Redirect/SLO
    sso: https://shibboleth.uni-bonn.de/idp/profile/SAML2/POST/SSO
  entity_categories:
  - DFN-AAI-IdP
  - http://aai.dfn.de/category/idm.nrw-member
  entity_id: https://shibboleth.uni-bonn.de/idp/shibboleth
  evidence: 'Metadata fetched from the institution''s own host (200, 12,145 bytes) and from the DFN-AAI aggregate (11,457 EntityDescriptors; this is the only uni-bonn.de entity in it), signed, on 2026-09-01. Observed in use: the BASIS student-information system (basis.uni-bonn.de) names Shibboleth and the Uni-ID on its sign-in page, and eCampus (ILIAS) offers SAML sign-in with the Uni-ID.'
  federation: DFN-AAI (Deutsches Forschungsnetz Authentication and Authorization Infrastructure)
  federation_metadata: https://mdq.aai.dfn.de/entities/
  metadata_url: https://shibboleth.uni-bonn.de/idp/shibboleth
  name: Shibboleth SAML 2.0 Identity Provider
  registration_authority: https://www.aai.dfn.de
  scope: uni-bonn.de
  type: saml2
  x-operator: institution
- evidence: 'Credentialed Dataverse endpoints answer anonymously with a token-shaped error rather than a wall: GET https://bonndata.uni-bonn.de/api/users/:me returned 400 {"status":"ERROR","message":"User with token null not found."} on 2026-09-01. Tokens are issued to authenticated bonndata accounts, which require a Uni-ID or an affiliated login; there is no public sign-up.'
  in: header
  name: Dataverse API token (X-Dataverse-key)
  parameter_name: X-Dataverse-key
  self_service: false
  type: api_key
  x-operator: institution
- evidence: 'The self-hosted GitLab at gitlab.uni-bonn.de serves its public project set anonymously but closes privileged endpoints: GET /api/v4/metadata and GET /api/v4/version both returned 401 {"message":"401 Unauthorized"} on 2026-09-01. Tokens require a university account.'
  in: header
  name: GitLab personal access token
  parameter_name: PRIVATE-TOKEN
  self_service: false
  type: api_key
  x-operator: institution
slug: university-of-bonn-authentication
source_filename: university-of-bonn-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-01'\nmethod: probed\nsource: >-\n  Live HTTP probes of uni-bonn.de authentication surfaces on 2026-09-01, plus the DFN-AAI\n  federation metadata aggregate (mdq.aai.dfn.de) and the university's own published IdP\n  metadata. No vendor authorization server is described here and no scheme is asserted\n  from documentation alone.\ndescription: >-\n  The University of Bonn operates its own authentication estate and publishes no public API\n  authorization server. Its one genuinely public API surface — the bonndata Dataverse read\n  subset and the two OAI-PMH endpoints — requires no credentials at all; everything\n  credentialed terminates at the institution's Shibboleth Identity Provider or at a\n  per-account token issued by an institutional service. There is no developer self-service\n  path: an unaffiliated developer cannot obtain a token for any Bonn system.\nsummary:\n  types:\n  - none\n  - saml2\n  - api_key\n  public_read_without_credentials: true\n\
  \  developer_self_service_tokens: false\nschemes:\n- name: No authentication (public read)\n  type: none\n  x-operator: institution\n  applies_to:\n  - https://bonndata.uni-bonn.de/api/search\n  - https://bonndata.uni-bonn.de/api/datasets\n  - https://bonndata.uni-bonn.de/api/info/version\n  - https://bonndata.uni-bonn.de/api/info/metrics/datasets\n  - https://bonndata.uni-bonn.de/oai\n  - https://bonndoc.ulb.uni-bonn.de/oai/request\n  - https://gitlab.uni-bonn.de/api/v4/projects\n  evidence: >-\n    All of the above returned 200 with real payloads to anonymous, un-credentialed requests\n    on 2026-09-01. The bonndata OpenAPI documents in this repo cover exactly this keyless\n    subset and nothing else.\n- name: Shibboleth SAML 2.0 Identity Provider\n  type: saml2\n  x-operator: institution\n  entity_id: https://shibboleth.uni-bonn.de/idp/shibboleth\n  metadata_url: https://shibboleth.uni-bonn.de/idp/shibboleth\n  scope: uni-bonn.de\n  federation: DFN-AAI (Deutsches Forschungsnetz Authentication\
  \ and Authorization Infrastructure)\n  federation_metadata: https://mdq.aai.dfn.de/entities/\n  registration_authority: https://www.aai.dfn.de\n  entity_categories:\n  - DFN-AAI-IdP\n  - http://aai.dfn.de/category/idm.nrw-member\n  bindings:\n  - urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect\n  - urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST\n  - urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST-SimpleSign\n  endpoints:\n    sso: https://shibboleth.uni-bonn.de/idp/profile/SAML2/POST/SSO\n    slo: https://shibboleth.uni-bonn.de/idp/profile/SAML2/Redirect/SLO\n    artifact_resolution: https://shibboleth.uni-bonn.de:8443/idp/profile/SAML2/SOAP/ArtifactResolution\n  evidence: >-\n    Metadata fetched from the institution's own host (200, 12,145 bytes) and from the\n    DFN-AAI aggregate (11,457 EntityDescriptors; this is the only uni-bonn.de entity in\n    it), signed, on 2026-09-01. Observed in use: the BASIS student-information system\n    (basis.uni-bonn.de) names Shibboleth and the\
  \ Uni-ID on its sign-in page, and eCampus\n    (ILIAS) offers SAML sign-in with the Uni-ID.\n- name: Dataverse API token (X-Dataverse-key)\n  type: api_key\n  x-operator: institution\n  in: header\n  parameter_name: X-Dataverse-key\n  self_service: false\n  evidence: >-\n    Credentialed Dataverse endpoints answer anonymously with a token-shaped error rather\n    than a wall: GET https://bonndata.uni-bonn.de/api/users/:me returned 400\n    {\"status\":\"ERROR\",\"message\":\"User with token null not found.\"} on 2026-09-01. Tokens\n    are issued to authenticated bonndata accounts, which require a Uni-ID or an affiliated\n    login; there is no public sign-up.\n- name: GitLab personal access token\n  type: api_key\n  x-operator: institution\n  in: header\n  parameter_name: PRIVATE-TOKEN\n  self_service: false\n  evidence: >-\n    The self-hosted GitLab at gitlab.uni-bonn.de serves its public project set anonymously\n    but closes privileged endpoints: GET /api/v4/metadata and GET /api/v4/version\
  \ both\n    returned 401 {\"message\":\"401 Unauthorized\"} on 2026-09-01. Tokens require a university\n    account.\nnot_found:\n- oauth2: >-\n    No OAuth 2.0 or OIDC authorization server, discovery document\n    (/.well-known/openid-configuration) or client-registration path was found on any\n    uni-bonn.de host.\n- developer_portal: >-\n    No developer portal, key-request form or API terms-of-use page exists; there is nothing\n    to sign up for.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-bonn/refs/heads/main/authentication/university-of-bonn-authentication.yml
summary_line: none/saml2/api_key · 4 schemes
tags:
- University
- Higher Education
- Education
- Germany
- Public Research University
- Research Data
- Open Data
- Open Science
- Institutional Repository
- Dataverse
- OAI-PMH
- Identity Federation
- Shibboleth
- DFN-AAI
- Research Computing
- Scholarly Publishing
---
