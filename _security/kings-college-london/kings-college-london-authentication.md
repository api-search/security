---
api_key_in: []
auth_types:
- http
- openIdConnect
- saml
- none
description: ''
kind: authentication
layout: security
method: probed
name: Kings College London Authentication
name_suffix: Authentication
oauth_flows: []
overview: King's College London secures its APIs with http, openIdConnect, saml, and none across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: King's College London
provider_slug: kings-college-london
scheme_count: 5
schemes:
- applies_to: https://ai.create.kcl.ac.uk/api/v1
  cors: 'access-control-allow-origin: * on the 401 response'
  description: 'The e-Research AI Hub exposes an OpenAI-compatible API that authenticates with an API key presented as `Authorization: Bearer <key>`. Keys are self-issued from the signed-in AI Hub dashboard; there is no public sign-up. Verified by probe: GET /api/v1/models with no header returns 401 `{"error":{"message":"Unauthorized — no bearer token provided","type": "invalid_request_error","param":null,"code":"invalid_api_key"}}`, and the same request with a syntactically valid but unknown bearer returns 401 with message "Unauthorized — invalid API key". The two distinct messages confirm the token is actually being validated rather than the header merely being required.'
  eligibility: researchers, students and staff of King's College London
  key_issuance: self-service, after institutional sign-in, from the AI Hub dashboard
  name: aiHubBearer
  operator: institution
  scheme: bearer
  sources:
  - https://ai.create.kcl.ac.uk/api/v1/models
  - https://docs.er.kcl.ac.uk/CREATE/ai_hub/
  type: http
- applies_to:
  - https://ai.create.kcl.ac.uk/
  - https://ai.create.kcl.ac.uk/docs
  - https://portal.er.kcl.ac.uk/
  description: 'Every human-facing e-Research surface sits behind Microsoft Entra ID. GET / and GET /docs on ai.create.kcl.ac.uk both return 200 carrying the Microsoft `BssoInterrupt` redirect document (aadcdn.msftauth.net assets, login.microsoftonline.com, autologon.microsoftazuread-sso.com), not the application. This is why the AI Hub''s own API reference could not be read for this profile: the documentation is authenticated, and the profile says so rather than guessing at its contents.'
  discovery: not published on a kcl.ac.uk host; the tenancy is Microsoft-hosted
  name: entraIdSso
  operator: institution
  sources:
  - https://ai.create.kcl.ac.uk/
  - https://portal.er.kcl.ac.uk/
  type: openIdConnect
- applies_to: https://kclidp.kcl.ac.uk/idp/shibboleth
  description: King's federated identity for external e-resources runs through the UK Access Management Federation and eduGAIN under entityID https://kclidp.kcl.ac.uk/idp/shibboleth, scoped to kcl.ac.uk, SIRTFI-certified and supporting the REFEDS Research and Scholarship entity category. Bindings offered are SAML 2.0 HTTP-Redirect and the legacy Shibboleth 1.0 AuthnRequest profile. Marked tenant because both SingleSignOnService Locations resolve to https://login.openathens.net/saml/2/sso/kcl.ac.uk/c/ukfed — OpenAthens operates the IdP on King's behalf.
  name: ukFederationSaml
  operator: tenant
  sources:
  - http://metadata.ukfederation.org.uk/ukfederation-metadata.xml
  - https://met.refeds.org/met/entity/https%3A%2F%2Fkclidp.kcl.ac.uk%2Fidp%2Fshibboleth/
  type: saml
- applies_to: CREATE Cloud OpenStack API
  description: 'Programmatic access to the CREATE Cloud OpenStack API requires three things, per King''s own documentation: an active OpenVPN session onto the e-Research network, an OpenStack application credential downloaded as clouds.yaml from the identity dashboard, and the KCL e-Research Root CA certificate added to the local trust store. cloud.er.kcl.ac.uk publishes no DNS record to the public internet, so none of this is reachable or verifiable from outside — recorded from documentation, not from a probe.'
  name: openAthensClientCertificate
  operator: institution
  scheme: mutual-tls
  sources:
  - https://docs.er.kcl.ac.uk/CREATE/cloud/openstack_api/
  type: http
- applies_to: https://kclpure.kcl.ac.uk/ws/oai
  description: The King's Research Portal OAI-PMH interface is fully open. Identify, ListMetadataFormats, ListSets and ListRecords all answer 200 with no credential of any kind, which is what an aggregator-facing harvesting endpoint should do.
  name: none
  operator: tenant
  sources:
  - https://kclpure.kcl.ac.uk/ws/oai?verb=Identify
  type: none
slug: kings-college-london-authentication
source_filename: kings-college-london-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-19'\nmethod: probed\nsource:\n- https://ai.create.kcl.ac.uk/api/v1/models\n- https://ai.create.kcl.ac.uk/\n- https://ai.create.kcl.ac.uk/docs\n- https://docs.er.kcl.ac.uk/CREATE/ai_hub/\n- https://docs.er.kcl.ac.uk/CREATE/cloud/openstack_api/\n- https://kclpure.kcl.ac.uk/ws/oai?verb=Identify\n- http://metadata.ukfederation.org.uk/ukfederation-metadata.xml\nnote: >-\n  King's publishes no OpenAPI, so nothing here is derived from a contract — every scheme below\n  was established by probing the live surface or by reading King's own e-Research documentation.\n  The institution runs three distinct authentication regimes and they do not share a credential:\n  an open unauthenticated metadata surface, a bearer-token API on the e-Research AI Hub, and\n  Microsoft Entra ID institutional SSO in front of everything with a user interface.\nsummary:\n  types:\n  - http\n  - openIdConnect\n  - saml\n  - none\nschemes:\n- name: aiHubBearer\n  type: http\n  scheme: bearer\n\
  \  applies_to: https://ai.create.kcl.ac.uk/api/v1\n  operator: institution\n  description: >-\n    The e-Research AI Hub exposes an OpenAI-compatible API that authenticates with an API key\n    presented as `Authorization: Bearer <key>`. Keys are self-issued from the signed-in AI Hub\n    dashboard; there is no public sign-up. Verified by probe: GET /api/v1/models with no header\n    returns 401 `{\"error\":{\"message\":\"Unauthorized — no bearer token provided\",\"type\":\n    \"invalid_request_error\",\"param\":null,\"code\":\"invalid_api_key\"}}`, and the same request with\n    a syntactically valid but unknown bearer returns 401 with message \"Unauthorized — invalid\n    API key\". The two distinct messages confirm the token is actually being validated rather\n    than the header merely being required.\n  key_issuance: self-service, after institutional sign-in, from the AI Hub dashboard\n  eligibility: researchers, students and staff of King's College London\n  cors: 'access-control-allow-origin:\
  \ * on the 401 response'\n  sources:\n  - https://ai.create.kcl.ac.uk/api/v1/models\n  - https://docs.er.kcl.ac.uk/CREATE/ai_hub/\n- name: entraIdSso\n  type: openIdConnect\n  applies_to:\n  - https://ai.create.kcl.ac.uk/\n  - https://ai.create.kcl.ac.uk/docs\n  - https://portal.er.kcl.ac.uk/\n  operator: institution\n  description: >-\n    Every human-facing e-Research surface sits behind Microsoft Entra ID. GET / and GET /docs on\n    ai.create.kcl.ac.uk both return 200 carrying the Microsoft `BssoInterrupt` redirect document\n    (aadcdn.msftauth.net assets, login.microsoftonline.com, autologon.microsoftazuread-sso.com),\n    not the application. This is why the AI Hub's own API reference could not be read for this\n    profile: the documentation is authenticated, and the profile says so rather than guessing at\n    its contents.\n  discovery: not published on a kcl.ac.uk host; the tenancy is Microsoft-hosted\n  sources:\n  - https://ai.create.kcl.ac.uk/\n  - https://portal.er.kcl.ac.uk/\n\
  - name: ukFederationSaml\n  type: saml\n  applies_to: https://kclidp.kcl.ac.uk/idp/shibboleth\n  operator: tenant\n  description: >-\n    King's federated identity for external e-resources runs through the UK Access Management\n    Federation and eduGAIN under entityID https://kclidp.kcl.ac.uk/idp/shibboleth, scoped to\n    kcl.ac.uk, SIRTFI-certified and supporting the REFEDS Research and Scholarship entity\n    category. Bindings offered are SAML 2.0 HTTP-Redirect and the legacy Shibboleth 1.0 AuthnRequest\n    profile. Marked tenant because both SingleSignOnService Locations resolve to\n    https://login.openathens.net/saml/2/sso/kcl.ac.uk/c/ukfed — OpenAthens operates the IdP on\n    King's behalf.\n  sources:\n  - http://metadata.ukfederation.org.uk/ukfederation-metadata.xml\n  - https://met.refeds.org/met/entity/https%3A%2F%2Fkclidp.kcl.ac.uk%2Fidp%2Fshibboleth/\n- name: openAthensClientCertificate\n  type: http\n  scheme: mutual-tls\n  applies_to: CREATE Cloud OpenStack API\n  operator:\
  \ institution\n  description: >-\n    Programmatic access to the CREATE Cloud OpenStack API requires three things, per King's own\n    documentation: an active OpenVPN session onto the e-Research network, an OpenStack\n    application credential downloaded as clouds.yaml from the identity dashboard, and the KCL\n    e-Research Root CA certificate added to the local trust store. cloud.er.kcl.ac.uk publishes\n    no DNS record to the public internet, so none of this is reachable or verifiable from\n    outside — recorded from documentation, not from a probe.\n  sources:\n  - https://docs.er.kcl.ac.uk/CREATE/cloud/openstack_api/\n- name: none\n  type: none\n  applies_to: https://kclpure.kcl.ac.uk/ws/oai\n  operator: tenant\n  description: >-\n    The King's Research Portal OAI-PMH interface is fully open. Identify, ListMetadataFormats,\n    ListSets and ListRecords all answer 200 with no credential of any kind, which is what an\n    aggregator-facing harvesting endpoint should do.\n  sources:\n\
  \  - https://kclpure.kcl.ac.uk/ws/oai?verb=Identify\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kings-college-london/refs/heads/main/authentication/kings-college-london-authentication.yml
summary_line: http/openIdConnect/saml/none · 5 schemes
tags:
- University
- Higher Education
- Education
- Russell Group
- United Kingdom
- London
- Research
- Research Computing
- Artificial Intelligence
- Institutional Repository
- Identity Federation
- OAI-PMH
- Library
---
