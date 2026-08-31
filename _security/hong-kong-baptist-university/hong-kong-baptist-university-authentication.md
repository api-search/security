---
api_key_in:
- header
auth_types:
- apiKey
- oauth2
- saml
- token
description: ''
kind: authentication
layout: security
method: probed
name: Hong Kong Baptist University Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hong Kong Baptist University secures its APIs with apiKey, oauth2, saml, and token across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Hong Kong Baptist University
provider_slug: hong-kong-baptist-university
scheme_count: 5
schemes:
- description: The HKBU GenAI Platform gateway takes an Azure-OpenAI-style api-key request header. A POST to https://genai.hkbu.edu.hk/general/rest/deployments/gpt-4o-mini/chat/completions ?api-version=2024-05-01-preview with no credential returns HTTP 401 {"message":"API key is missing or invalid.","error":"Unauthorized","statusCode":401}. The same POST carrying an api-key header returns a different HTTP 401, {"message":"API key validation failed due to an internal error.",...}, which is what identifies api-key as the credential channel rather than Authorization or x-api-key — both of those produce the "missing or invalid" message instead. No self-service issuance path is published; keys are obtained through institutional affiliation.
  evidence:
  - status: 401
    url: https://genai.hkbu.edu.hk/general/rest/deployments/gpt-4o-mini/chat/completions?api-version=2024-05-01-preview
  in: header
  name: genai-api-key
  operator: institution
  parameter: api-key
  surface: hong-kong-baptist-university:genai-platform-api
  type: apiKey
- description: IMS LTI 1.3 Advantage service authentication. The token endpoint returns HTTP 400 {"error":"invalid_request"} to a bare call, and the platform key set at /mod/lti/certs.php returns HTTP 200 with a single RSA RS256 signing key (kid 233f84e26d75aa18234e). Tools registered with HKBU exchange a signed JWT assertion for an access token here.
  evidence:
  - status: 400
    url: https://buelearning.hkbu.edu.hk/mod/lti/token.php
  - status: 200
    url: https://buelearning.hkbu.edu.hk/mod/lti/certs.php
  flow: clientCredentials
  jwksUrl: https://buelearning.hkbu.edu.hk/mod/lti/certs.php
  name: moodle-lti-oauth2-client-credentials
  operator: institution
  surface: hong-kong-baptist-university:moodle-lti-platform
  tokenUrl: https://buelearning.hkbu.edu.hk/mod/lti/token.php
  type: oauth2
- description: Moodle Web Services is enabled on the HKBU Moodle. A call to /webservice/rest/server.php?wsfunction=core_webservice_get_site_info&moodlewsrestformat=json with no token returns HTTP 200 carrying Moodle's own error envelope, {"exception":"core\\exception\\moodle_exception","errorcode":"invalidtoken", "message":"Invalid token - token not found"} — an enabled service refusing a credential, not a disabled one 404ing. Tokens are issued per user through institutional login.
  evidence:
  - status: 200
    url: https://buelearning.hkbu.edu.hk/webservice/rest/server.php?wsfunction=core_webservice_get_site_info&moodlewsrestformat=json
  in: query
  name: moodle-webservice-token
  operator: institution
  parameter: wstoken
  surface: hong-kong-baptist-university:moodle-lti-platform
  type: token
- description: 'HKBU''s own SAML 2.0 / Shibboleth identity provider is the institution''s federated authentication surface, and it is the one credential system here whose metadata is public. Bindings: SAML2 HTTP-POST, HTTP-POST-SimpleSign and HTTP-Redirect for SSO; SOAP on port 8443 for ArtifactResolution and AttributeQuery; SAML 1.1 SOAP equivalents; HTTP-Redirect SingleLogout. Attribute release is scoped to hkbu.edu.hk. Registered in eduGAIN by the Hong Kong Access Federation. Technical contact published in the metadata: jackkwok@hkbu.edu.hk.'
  entityId: https://buidp01.hkbu.edu.hk/idp/shibboleth
  evidence:
  - status: 200
    url: https://buidp01.hkbu.edu.hk/idp/shibboleth
  name: hkbu-shibboleth-idp
  operator: institution
  surface: hong-kong-baptist-university:identity-federation
  type: saml
- credited: false
  description: 'The Elsevier Pure Web Service running under HKBU''s name at scholars.hkbu.edu.hk/ws/api is api-key gated — /ws/api/524/openapi.yaml returns HTTP 401 without one. Recorded because the tenancy is a real institutional fact, and explicitly NOT credited to HKBU: the scheme, the contract and the implementation are Elsevier''s.'
  evidence:
  - status: 401
    url: https://scholars.hkbu.edu.hk/ws/api/524/openapi.yaml
  in: header
  name: pure-api-key
  operator: tenant
  parameter: api-key
  surface: hong-kong-baptist-university:scholars-pure-tenancy
  type: apiKey
slug: hong-kong-baptist-university-authentication
source_filename: hong-kong-baptist-university-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: probed\nsource: >-\n  Live credential probes of HKBU-operated hosts on 2026-08-30. This file replaces the\n  2026-07-11 version, which was derived from Elsevier's Pure OpenAPI and therefore described\n  Elsevier's authentication, not HKBU's.\nnote: >-\n  HKBU publishes no security schemes in any contract of its own, because it publishes no\n  contract of its own. Every scheme below was established by sending a request and reading the\n  rejection. Nothing here is inferred from documentation.\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  - saml\n  - token\n  api_key_in:\n  - header\nschemes:\n- name: genai-api-key\n  type: apiKey\n  in: header\n  parameter: api-key\n  operator: institution\n  surface: hong-kong-baptist-university:genai-platform-api\n  description: >-\n    The HKBU GenAI Platform gateway takes an Azure-OpenAI-style api-key request header. A POST\n    to https://genai.hkbu.edu.hk/general/rest/deployments/gpt-4o-mini/chat/completions\n\
  \    ?api-version=2024-05-01-preview with no credential returns HTTP 401\n    {\"message\":\"API key is missing or invalid.\",\"error\":\"Unauthorized\",\"statusCode\":401}. The\n    same POST carrying an api-key header returns a different HTTP 401,\n    {\"message\":\"API key validation failed due to an internal error.\",...}, which is what\n    identifies api-key as the credential channel rather than Authorization or x-api-key —\n    both of those produce the \"missing or invalid\" message instead. No self-service issuance\n    path is published; keys are obtained through institutional affiliation.\n  evidence:\n  - url: https://genai.hkbu.edu.hk/general/rest/deployments/gpt-4o-mini/chat/completions?api-version=2024-05-01-preview\n    status: 401\n- name: moodle-lti-oauth2-client-credentials\n  type: oauth2\n  flow: clientCredentials\n  operator: institution\n  surface: hong-kong-baptist-university:moodle-lti-platform\n  tokenUrl: https://buelearning.hkbu.edu.hk/mod/lti/token.php\n \
  \ jwksUrl: https://buelearning.hkbu.edu.hk/mod/lti/certs.php\n  description: >-\n    IMS LTI 1.3 Advantage service authentication. The token endpoint returns HTTP 400\n    {\"error\":\"invalid_request\"} to a bare call, and the platform key set at /mod/lti/certs.php\n    returns HTTP 200 with a single RSA RS256 signing key (kid 233f84e26d75aa18234e). Tools\n    registered with HKBU exchange a signed JWT assertion for an access token here.\n  evidence:\n  - url: https://buelearning.hkbu.edu.hk/mod/lti/token.php\n    status: 400\n  - url: https://buelearning.hkbu.edu.hk/mod/lti/certs.php\n    status: 200\n- name: moodle-webservice-token\n  type: token\n  in: query\n  parameter: wstoken\n  operator: institution\n  surface: hong-kong-baptist-university:moodle-lti-platform\n  description: >-\n    Moodle Web Services is enabled on the HKBU Moodle. A call to\n    /webservice/rest/server.php?wsfunction=core_webservice_get_site_info&moodlewsrestformat=json\n    with no token returns HTTP 200 carrying\
  \ Moodle's own error envelope,\n    {\"exception\":\"core\\\\exception\\\\moodle_exception\",\"errorcode\":\"invalidtoken\",\n    \"message\":\"Invalid token - token not found\"} — an enabled service refusing a credential,\n    not a disabled one 404ing. Tokens are issued per user through institutional login.\n  evidence:\n  - url: https://buelearning.hkbu.edu.hk/webservice/rest/server.php?wsfunction=core_webservice_get_site_info&moodlewsrestformat=json\n    status: 200\n- name: hkbu-shibboleth-idp\n  type: saml\n  operator: institution\n  surface: hong-kong-baptist-university:identity-federation\n  entityId: https://buidp01.hkbu.edu.hk/idp/shibboleth\n  description: >-\n    HKBU's own SAML 2.0 / Shibboleth identity provider is the institution's federated\n    authentication surface, and it is the one credential system here whose metadata is public.\n    Bindings: SAML2 HTTP-POST, HTTP-POST-SimpleSign and HTTP-Redirect for SSO; SOAP on port 8443\n    for ArtifactResolution and AttributeQuery;\
  \ SAML 1.1 SOAP equivalents; HTTP-Redirect\n    SingleLogout. Attribute release is scoped to hkbu.edu.hk. Registered in eduGAIN by the Hong\n    Kong Access Federation. Technical contact published in the metadata: jackkwok@hkbu.edu.hk.\n  evidence:\n  - url: https://buidp01.hkbu.edu.hk/idp/shibboleth\n    status: 200\n- name: pure-api-key\n  type: apiKey\n  in: header\n  parameter: api-key\n  operator: tenant\n  credited: false\n  surface: hong-kong-baptist-university:scholars-pure-tenancy\n  description: >-\n    The Elsevier Pure Web Service running under HKBU's name at scholars.hkbu.edu.hk/ws/api is\n    api-key gated — /ws/api/524/openapi.yaml returns HTTP 401 without one. Recorded because the\n    tenancy is a real institutional fact, and explicitly NOT credited to HKBU: the scheme,\n    the contract and the implementation are Elsevier's.\n  evidence:\n  - url: https://scholars.hkbu.edu.hk/ws/api/524/openapi.yaml\n    status: 401\nnegative_probes:\n- url: https://genai.hkbu.edu.hk/.well-known/openid-configuration\n\
  \  status: 404\n  note: No OIDC discovery document; the GenAI gateway is api-key only.\n- url: https://genai.hkbu.edu.hk/scim/v2/Users\n  status: 404\n  note: No SCIM provisioning endpoint.\n- url: https://buelearning.hkbu.edu.hk/scim/v2/Users\n  status: 404\n  note: No SCIM provisioning endpoint on the LMS either.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hong-kong-baptist-university/refs/heads/main/authentication/hong-kong-baptist-university-authentication.yml
summary_line: apiKey/oauth2/saml/token · 5 schemes
tags:
- University
- Higher Education
- Education
- Hong Kong
- UGC-Funded
- Identity Federation
- Shibboleth
- SAML
- eduGAIN
- Learning Management
- LTI
- Artificial Intelligence
- Research Information
- Elsevier Pure
---
