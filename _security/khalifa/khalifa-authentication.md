---
api_key_in: []
api_specs:
- filename: khalifa-khazna-oai-pmh-openapi.yml
  format: yaml
  label: Khazna OAI-PMH Repository
  slug: khazna-oai-pmh
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/khalifa/refs/heads/main/openapi/khalifa-khazna-oai-pmh-openapi.yml
auth_types:
- none
- oauth2
- saml
- apiKey
description: ''
kind: authentication
layout: security
method: probed
name: Khalifa Authentication
name_suffix: Authentication
oauth_flows: []
overview: Khalifa University secures its APIs with none, oauth2, saml, and apiKey across 7 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Khalifa University
provider_slug: khalifa
scheme_count: 7
schemes:
- applies_to: https://khazna.ku.ac.ae/ws/oai
  description: 'The Khazna OAI-PMH base URL is open and anonymous, as OAI-PMH 2.0 requires. Probed 2026-09-01: ?verb=Identify, ?verb=ListMetadataFormats and ?verb=ListSets all returned HTTP 200 with no credential of any kind.'
  evidence:
    status: 200
    url: https://khazna.ku.ac.ae/ws/oai?verb=Identify
  name: KhaznaOaiPmhPublic
  operator: institution
  type: none
- applies_to: https://www.ku.ac.ae/wp-json
  description: 'The WordPress REST API on the university''s own web host answers its discovery root anonymously (HTTP 200, 17 namespaces, 202 routes, name "Khalifa University"), and a subset of routes return real data without credentials — wp/v2/search and tribe/events/v1/* were both HTTP 200 on 2026-09-01. The core wp/v2 collection routes are deliberately closed: they return HTTP 401 with code "itsec_rest_api_access_restricted" (the iThemes/Solid Security REST restriction). Write access is gated behind WordPress application passwords, authorization at https://www.ku.ac.ae/wp-admin/authorize-application.php, which is not usable by the public.'
  evidence:
    status: 200
    url: https://www.ku.ac.ae/wp-json/wp/v2/search?search=research&per_page=1
  name: KuWebRestPartiallyOpen
  operator: institution
  type: none
- applies_to: https://login.microsoftonline.com/ku.ac.ae/v2.0
  description: Khalifa University's own Microsoft Entra ID tenant (08fe1c0a-19f5-4f24-a662-fdd5dd460025) is the OpenID Connect issuer for the ku.ac.ae namespace. The discovery document is public and machine-readable; obtaining a token requires an institution account. This is the strongest institution-operated identity surface Khalifa publishes.
  evidence:
    status: 200
    url: https://login.microsoftonline.com/ku.ac.ae/v2.0/.well-known/openid-configuration
  name: EntraIdOidc
  operator: institution
  type: oauth2
- applies_to: https://login.microsoftonline.com/08fe1c0a-19f5-4f24-a662-fdd5dd460025/saml2
  description: 'SAML 2.0 single sign-on for institution systems, issued by the same tenant. Observed in production: https://elearn.ku.ac.ae/ redirects to the tenant''s /saml2 endpoint with a SAMLRequest, and https://portal.ku.ac.ae/ and https://kubee.ku.ac.ae/ redirect to its WS-Federation endpoint with wtrealm http://adfs.ku.ac.ae/adfs/services/trust. Federation metadata is published and returns HTTP 200.'
  evidence:
    status: 200
    url: https://login.microsoftonline.com/ku.ac.ae/federationmetadata/2007-06/federationmetadata.xml
  name: EntraIdSaml
  operator: institution
  type: saml
- applies_to: https://khazna.ku.ac.ae/ws/api
  description: 'NOT KHALIFA''S SCHEME — recorded so a later run does not rediscover it and mistake it for the institution''s. The Elsevier Pure Web Service on the Khazna host declares `security: [{api-key: []}]` in its own contract (info.title "Pure API", version 5.36.2-1, info.contact.email pure-support@elsevier.com, servers "- url: /ws/api"). The contract is Elsevier''s product spec served under Khalifa''s hostname; the versioned and swagger paths (/ws/api/524/openapi.yaml, /ws/api/swagger.json) return HTTP 401. Keys are issued by the institution''s Pure administrators, but the auth model is the vendor''s.'
  evidence:
    status: 200
    url: https://khazna.ku.ac.ae/ws/api/openapi.yaml
  name: PureWebServiceApiKey
  operator: vendor
  type: apiKey
- applies_to: https://khalifauni.blackboard.com/learn/api/public/v1
  description: NOT KHALIFA'S SCHEME. The Blackboard Learn REST API on Khalifa's tenant is protected by Anthology's three-legged OAuth 2.0 with developer keys registered in the Blackboard Developer Portal. Only /learn/api/public/v1/system/version is anonymous, which is what confirmed the tenant is live. Recorded as the vendor's.
  evidence:
    status: 200
    url: https://khalifauni.blackboard.com/learn/api/public/v1/system/version
  name: BlackboardLearnOauth2
  operator: vendor
  type: oauth2
- applies_to: https://lgapi-us.libapps.com
  description: NOT KHALIFA'S SCHEME. LibGuides/LibAnswers/LibCal API access for the kustar Springshare account is issued per site by Springshare and keyed to their platform. Recorded as the vendor's; the tenancy itself is real and is recorded in apis.yml.
  evidence:
    status: 200
    url: https://library.ku.ac.ae/lib
  name: SpringshareLibAppsApiKey
  operator: vendor
  type: apiKey
slug: khalifa-authentication
source_filename: khalifa-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-01'\nmethod: probed\nsource: >-\n  Live probes 2026-09-01 of every surface attributed to Khalifa University, plus\n  openapi/khalifa-khazna-oai-pmh-openapi.yml. Each scheme records the operator of the thing it\n  protects, because most of Khalifa's authenticated surface area belongs to vendors it rents.\nprovider: Khalifa University\nproviderId: khalifa\nsummary:\n  types:\n  - none\n  - oauth2\n  - saml\n  - apiKey\n  institution_operated_public_apis_requiring_no_auth: 2\nschemes:\n- name: KhaznaOaiPmhPublic\n  type: none\n  operator: institution\n  applies_to: https://khazna.ku.ac.ae/ws/oai\n  description: >-\n    The Khazna OAI-PMH base URL is open and anonymous, as OAI-PMH 2.0 requires. Probed\n    2026-09-01: ?verb=Identify, ?verb=ListMetadataFormats and ?verb=ListSets all returned HTTP\n    200 with no credential of any kind.\n  evidence:\n    url: https://khazna.ku.ac.ae/ws/oai?verb=Identify\n    status: 200\n- name: KuWebRestPartiallyOpen\n  type:\
  \ none\n  operator: institution\n  applies_to: https://www.ku.ac.ae/wp-json\n  description: >-\n    The WordPress REST API on the university's own web host answers its discovery root\n    anonymously (HTTP 200, 17 namespaces, 202 routes, name \"Khalifa University\"), and a subset of\n    routes return real data without credentials — wp/v2/search and tribe/events/v1/* were both\n    HTTP 200 on 2026-09-01. The core wp/v2 collection routes are deliberately closed: they return\n    HTTP 401 with code \"itsec_rest_api_access_restricted\" (the iThemes/Solid Security REST\n    restriction). Write access is gated behind WordPress application passwords, authorization at\n    https://www.ku.ac.ae/wp-admin/authorize-application.php, which is not usable by the public.\n  evidence:\n    url: https://www.ku.ac.ae/wp-json/wp/v2/search?search=research&per_page=1\n    status: 200\n- name: EntraIdOidc\n  type: oauth2\n  operator: institution\n  applies_to: https://login.microsoftonline.com/ku.ac.ae/v2.0\n\
  \  description: >-\n    Khalifa University's own Microsoft Entra ID tenant (08fe1c0a-19f5-4f24-a662-fdd5dd460025) is\n    the OpenID Connect issuer for the ku.ac.ae namespace. The discovery document is public and\n    machine-readable; obtaining a token requires an institution account. This is the strongest\n    institution-operated identity surface Khalifa publishes.\n  evidence:\n    url: https://login.microsoftonline.com/ku.ac.ae/v2.0/.well-known/openid-configuration\n    status: 200\n- name: EntraIdSaml\n  type: saml\n  operator: institution\n  applies_to: https://login.microsoftonline.com/08fe1c0a-19f5-4f24-a662-fdd5dd460025/saml2\n  description: >-\n    SAML 2.0 single sign-on for institution systems, issued by the same tenant. Observed in\n    production: https://elearn.ku.ac.ae/ redirects to the tenant's /saml2 endpoint with a\n    SAMLRequest, and https://portal.ku.ac.ae/ and https://kubee.ku.ac.ae/ redirect to its\n    WS-Federation endpoint with wtrealm http://adfs.ku.ac.ae/adfs/services/trust.\
  \ Federation\n    metadata is published and returns HTTP 200.\n  evidence:\n    url: https://login.microsoftonline.com/ku.ac.ae/federationmetadata/2007-06/federationmetadata.xml\n    status: 200\n- name: PureWebServiceApiKey\n  type: apiKey\n  operator: vendor\n  applies_to: https://khazna.ku.ac.ae/ws/api\n  description: >-\n    NOT KHALIFA'S SCHEME — recorded so a later run does not rediscover it and mistake it for the\n    institution's. The Elsevier Pure Web Service on the Khazna host declares\n    `security: [{api-key: []}]` in its own contract (info.title \"Pure API\", version 5.36.2-1,\n    info.contact.email pure-support@elsevier.com, servers \"- url: /ws/api\"). The contract is\n    Elsevier's product spec served under Khalifa's hostname; the versioned and swagger paths\n    (/ws/api/524/openapi.yaml, /ws/api/swagger.json) return HTTP 401. Keys are issued by the\n    institution's Pure administrators, but the auth model is the vendor's.\n  evidence:\n    url: https://khazna.ku.ac.ae/ws/api/openapi.yaml\n\
  \    status: 200\n- name: BlackboardLearnOauth2\n  type: oauth2\n  operator: vendor\n  applies_to: https://khalifauni.blackboard.com/learn/api/public/v1\n  description: >-\n    NOT KHALIFA'S SCHEME. The Blackboard Learn REST API on Khalifa's tenant is protected by\n    Anthology's three-legged OAuth 2.0 with developer keys registered in the Blackboard Developer\n    Portal. Only /learn/api/public/v1/system/version is anonymous, which is what confirmed the\n    tenant is live. Recorded as the vendor's.\n  evidence:\n    url: https://khalifauni.blackboard.com/learn/api/public/v1/system/version\n    status: 200\n- name: SpringshareLibAppsApiKey\n  type: apiKey\n  operator: vendor\n  applies_to: https://lgapi-us.libapps.com\n  description: >-\n    NOT KHALIFA'S SCHEME. LibGuides/LibAnswers/LibCal API access for the kustar Springshare\n    account is issued per site by Springshare and keyed to their platform. Recorded as the\n    vendor's; the tenancy itself is real and is recorded in apis.yml.\n\
  \  evidence:\n    url: https://library.ku.ac.ae/lib\n    status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/khalifa/refs/heads/main/authentication/khalifa-authentication.yml
summary_line: none/oauth2/saml/apiKey · 7 schemes
tags:
- University
- Higher Education
- Education
- Research
- Research Data
- Research Repository
- Identity Federation
- OAI-PMH
- Robotics
- United Arab Emirates
- Abu Dhabi
---
