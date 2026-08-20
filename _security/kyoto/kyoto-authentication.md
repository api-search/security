---
api_key_in: []
api_specs:
- filename: kyoto-oai-pmh-api-openapi.yml
  format: yaml
  label: KURENAI OAI-PMH API
  slug: kyoto-oai-pmh-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kyoto/refs/heads/main/openapi/kyoto-oai-pmh-api-openapi.yml
- filename: kyoto-rest-api-openapi.yml
  format: yaml
  label: KURENAI DSpace REST API
  slug: kyoto-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kyoto/refs/heads/main/openapi/kyoto-rest-api-openapi.yml
- filename: kyoto-lms-api-openapi.yml
  format: yaml
  label: PandA Learning Support System API (Sakai Entity Broker + IMS LTI)
  slug: kyoto-lms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kyoto/refs/heads/main/openapi/kyoto-lms-api-openapi.yml
auth_types:
- none
- saml
- session
description: ''
kind: authentication
layout: security
method: probed
name: Kyoto Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kyoto University secures its APIs with none, saml, and session across 6 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Kyoto University
provider_slug: kyoto
scheme_count: 6
schemes:
- applies_to: https://repository.kulib.kyoto-u.ac.jp
  description: KURENAI's public surfaces are anonymous reads. The DSpace 7.6 REST root, the community and collection listings, and the whole OAI-PMH 2.0 endpoint answer with no credential. Item submission and administrative endpoints require a repository account and were not exercised.
  evidence:
    status: 200
    url: https://repository.kulib.kyoto-u.ac.jp/server/api/core/communities
  name: KurenaiPublicRead
  operator: institution
  type: none
- applies_to: https://repository.kulib.kyoto-u.ac.jp/server/oai/request
  description: OAI-PMH 2.0 harvesting is open by design; verb=Identify, verb=ListMetadataFormats and verb=ListRecords all answer anonymously.
  evidence:
    status: 200
    url: https://repository.kulib.kyoto-u.ac.jp/server/oai/request?verb=Identify
  name: KurenaiOaiPmhPublic
  operator: institution
  type: none
- applies_to: https://panda.ecs.kyoto-u.ac.jp/direct
  description: The Sakai Entity Broker answers anonymously on the public prefixes. /direct/tool.json returns the full 96-entry tool registry; /direct/site.json, /direct/syllabus.json, /direct/announcement.json, /direct/assignment.json, /direct/calendar.json, /direct/content.json and /direct/lti.json return their envelope with an empty collection, and /direct/session.json returns a session object with null id, userId and userEid. No course, roster or personal data is exposed without a session.
  evidence:
    status: 200
    url: https://panda.ecs.kyoto-u.ac.jp/direct/tool.json
  name: PandaAnonymousRead
  operator: institution
  type: none
- additional_evidence:
  - status: 401
    url: https://panda.ecs.kyoto-u.ac.jp/direct/poll.json
  - note: Human login entry point published by the IIMC.
    status: 200
    url: https://panda.ecs.kyoto-u.ac.jp/portal/login
  applies_to: https://panda.ecs.kyoto-u.ac.jp
  description: 'Privileged PandA entities require an authenticated Sakai session established through the university login (ECS-ID for students, SPS-ID for faculty and staff), which is itself federated through the IIMC Shibboleth IdP with multi-factor authentication. The boundary is enforced and differentiated: /direct/poll.json returns 401, /direct/user.json returns 403, and /direct/membership.json returns 400 when required parameters are absent.'
  evidence:
    status: 403
    url: https://panda.ecs.kyoto-u.ac.jp/direct/user.json
  name: PandaSakaiSession
  operator: institution
  type: session
- additional_evidence:
  - note: Kyoto's IdP is present in the GakuNin aggregate metadata as entityID https://authidp1.iimc.kyoto-u.ac.jp/idp/shibboleth.
    status: 200
    url: https://metadata.gakunin.nii.ac.jp/gakunin-metadata.xml
  - note: IIMC multi-factor authentication documentation.
    status: 200
    url: https://www.iimc.kyoto-u.ac.jp/en/services/account/mfa
  applies_to: https://authidp1.iimc.kyoto-u.ac.jp/idp/shibboleth
  description: Kyoto University operates its own Shibboleth SAML 2.0 Identity Provider, run by the Institute for Information Management and Communication and registered in GakuNin, the Japanese academic access management federation (National Institute of Informatics), which participates in eduGAIN. Metadata is public and machine-readable at the canonical /idp/shibboleth location and declares <shibmd:Scope>kyoto-u.ac.jp</shibmd:Scope>. Single sign-on is offered over SAML 2.0 HTTP-POST (https://authidp1.iimc.kyoto-u.ac.jp/idp/profile/SAML2/POST/SSO), SAML 2.0 HTTP-Redirect (.../SAML2/Redirect/SSO) and the legacy Shibboleth 1.0 AuthnRequest profile (.../profile/Shibboleth/SSO). University accounts are SPS-ID (faculty/staff) and ECS-ID (students), with multi-factor authentication documented by the IIMC. Service-provider connections to the federation require committee approval — this is institutional SSO infrastructure, not a self-service API.
  entity_id: https://authidp1.iimc.kyoto-u.ac.jp/idp/shibboleth
  evidence:
    content_type: application/xml
    status: 200
    url: https://authidp1.iimc.kyoto-u.ac.jp/idp/shibboleth
  local_copy: authentication/kyoto-saml-idp-metadata.xml
  name: KyotoShibbolethIdP
  operator: institution
  type: saml
- applies_to: https://web.kudpc.kyoto-u.ac.jp/shibboleth-sp
  description: The supercomputer systems of the Academic Center for Computing and Media Studies are fronted by a Kyoto University-operated Shibboleth service provider registered in GakuNin, with five AssertionConsumerService endpoints (SAML 2.0 HTTP-POST, POST-SimpleSign and HTTP-Artifact, plus the SAML 1.0 browser-post and artifact profiles). Contact consult@kudpc.kyoto-u.ac.jp. This is how researchers reach institution-operated research computing, and it is the access layer for that service rather than a data API.
  entity_id: https://web.kudpc.kyoto-u.ac.jp/shibboleth-sp
  evidence:
    note: Entity present in the GakuNin aggregate. The SP's own /Shibboleth.sso/Metadata handler returns 500 to a direct anonymous request (2026-08-19), so the federation aggregate is the citable copy.
    status: 200
    url: https://metadata.gakunin.nii.ac.jp/gakunin-metadata.xml
  name: KudpcShibbolethSP
  operator: institution
  type: saml
slug: kyoto-authentication
source_filename: kyoto-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-19'\nmethod: probed\nsource: >-\n  Live probes on 2026-08-19 of every surface attributed to Kyoto University, plus\n  openapi/kyoto-lms-api-openapi.yml, openapi/kyoto-rest-api-openapi.yml and\n  openapi/kyoto-oai-pmh-api-openapi.yml. No credential was sent to any host and no authentication\n  was attempted; gated surfaces are described by the status they return to an anonymous caller.\nprovider: Kyoto University\nproviderId: kyoto\nsummary:\n  types:\n  - none\n  - saml\n  - session\n  institution_operated_public_apis_requiring_no_auth: 3\n  oauth2: false\n  api_keys: false\nschemes:\n- name: KurenaiPublicRead\n  type: none\n  operator: institution\n  applies_to: https://repository.kulib.kyoto-u.ac.jp\n  description: >-\n    KURENAI's public surfaces are anonymous reads. The DSpace 7.6 REST root, the community and\n    collection listings, and the whole OAI-PMH 2.0 endpoint answer with no credential. Item\n    submission and administrative endpoints require\
  \ a repository account and were not exercised.\n  evidence:\n    url: https://repository.kulib.kyoto-u.ac.jp/server/api/core/communities\n    status: 200\n- name: KurenaiOaiPmhPublic\n  type: none\n  operator: institution\n  applies_to: https://repository.kulib.kyoto-u.ac.jp/server/oai/request\n  description: >-\n    OAI-PMH 2.0 harvesting is open by design; verb=Identify, verb=ListMetadataFormats and\n    verb=ListRecords all answer anonymously.\n  evidence:\n    url: https://repository.kulib.kyoto-u.ac.jp/server/oai/request?verb=Identify\n    status: 200\n- name: PandaAnonymousRead\n  type: none\n  operator: institution\n  applies_to: https://panda.ecs.kyoto-u.ac.jp/direct\n  description: >-\n    The Sakai Entity Broker answers anonymously on the public prefixes. /direct/tool.json returns\n    the full 96-entry tool registry; /direct/site.json, /direct/syllabus.json,\n    /direct/announcement.json, /direct/assignment.json, /direct/calendar.json, /direct/content.json\n    and /direct/lti.json\
  \ return their envelope with an empty collection, and /direct/session.json\n    returns a session object with null id, userId and userEid. No course, roster or personal data is\n    exposed without a session.\n  evidence:\n    url: https://panda.ecs.kyoto-u.ac.jp/direct/tool.json\n    status: 200\n- name: PandaSakaiSession\n  type: session\n  operator: institution\n  applies_to: https://panda.ecs.kyoto-u.ac.jp\n  description: >-\n    Privileged PandA entities require an authenticated Sakai session established through the\n    university login (ECS-ID for students, SPS-ID for faculty and staff), which is itself federated\n    through the IIMC Shibboleth IdP with multi-factor authentication. The boundary is enforced and\n    differentiated: /direct/poll.json returns 401, /direct/user.json returns 403, and\n    /direct/membership.json returns 400 when required parameters are absent.\n  evidence:\n    url: https://panda.ecs.kyoto-u.ac.jp/direct/user.json\n    status: 403\n  additional_evidence:\n\
  \  - url: https://panda.ecs.kyoto-u.ac.jp/direct/poll.json\n    status: 401\n  - url: https://panda.ecs.kyoto-u.ac.jp/portal/login\n    status: 200\n    note: Human login entry point published by the IIMC.\n- name: KyotoShibbolethIdP\n  type: saml\n  operator: institution\n  applies_to: https://authidp1.iimc.kyoto-u.ac.jp/idp/shibboleth\n  entity_id: https://authidp1.iimc.kyoto-u.ac.jp/idp/shibboleth\n  description: >-\n    Kyoto University operates its own Shibboleth SAML 2.0 Identity Provider, run by the Institute\n    for Information Management and Communication and registered in GakuNin, the Japanese academic\n    access management federation (National Institute of Informatics), which participates in eduGAIN.\n    Metadata is public and machine-readable at the canonical /idp/shibboleth location and declares\n    <shibmd:Scope>kyoto-u.ac.jp</shibmd:Scope>. Single sign-on is offered over SAML 2.0 HTTP-POST\n    (https://authidp1.iimc.kyoto-u.ac.jp/idp/profile/SAML2/POST/SSO), SAML 2.0\
  \ HTTP-Redirect\n    (.../SAML2/Redirect/SSO) and the legacy Shibboleth 1.0 AuthnRequest profile\n    (.../profile/Shibboleth/SSO). University accounts are SPS-ID (faculty/staff) and ECS-ID\n    (students), with multi-factor authentication documented by the IIMC. Service-provider\n    connections to the federation require committee approval — this is institutional SSO\n    infrastructure, not a self-service API.\n  evidence:\n    url: https://authidp1.iimc.kyoto-u.ac.jp/idp/shibboleth\n    status: 200\n    content_type: application/xml\n  additional_evidence:\n  - url: https://metadata.gakunin.nii.ac.jp/gakunin-metadata.xml\n    status: 200\n    note: Kyoto's IdP is present in the GakuNin aggregate metadata as entityID https://authidp1.iimc.kyoto-u.ac.jp/idp/shibboleth.\n  - url: https://www.iimc.kyoto-u.ac.jp/en/services/account/mfa\n    status: 200\n    note: IIMC multi-factor authentication documentation.\n  local_copy: authentication/kyoto-saml-idp-metadata.xml\n- name: KudpcShibbolethSP\n\
  \  type: saml\n  operator: institution\n  applies_to: https://web.kudpc.kyoto-u.ac.jp/shibboleth-sp\n  entity_id: https://web.kudpc.kyoto-u.ac.jp/shibboleth-sp\n  description: >-\n    The supercomputer systems of the Academic Center for Computing and Media Studies are fronted by\n    a Kyoto University-operated Shibboleth service provider registered in GakuNin, with five\n    AssertionConsumerService endpoints (SAML 2.0 HTTP-POST, POST-SimpleSign and HTTP-Artifact, plus\n    the SAML 1.0 browser-post and artifact profiles). Contact consult@kudpc.kyoto-u.ac.jp. This is\n    how researchers reach institution-operated research computing, and it is the access layer for\n    that service rather than a data API.\n  evidence:\n    url: https://metadata.gakunin.nii.ac.jp/gakunin-metadata.xml\n    status: 200\n    note: >-\n      Entity present in the GakuNin aggregate. The SP's own /Shibboleth.sso/Metadata handler returns\n      500 to a direct anonymous request (2026-08-19), so the federation\
  \ aggregate is the citable copy.\nnotes: >-\n  Kyoto University publishes no OAuth 2.0 authorization server, no API key programme and no\n  developer registration of any kind. Every institution-operated public interface it runs is either\n  fully anonymous (KURENAI REST, KURENAI OAI-PMH, the PandA public prefixes) or gated behind\n  university SSO. This file replaces nothing: before 2026-08-19 the repository carried no\n  authentication artifact at all.\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kyoto/refs/heads/main/authentication/kyoto-authentication.yml
summary_line: none/saml/session · 6 schemes
tags:
- University
- Higher Education
- Education
- Japan
- National University
- Research Repository
- Research Data
- Identity Federation
- Learning Management
- Open Access
- Research Computing
- Scholarly
---
