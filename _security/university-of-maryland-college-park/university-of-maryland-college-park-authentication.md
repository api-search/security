---
api_key_in: []
api_specs:
- filename: university-of-maryland-college-park-libraries-website-tools-openapi.yml
  format: yaml
  label: UMD Libraries Website Tools API
  slug: libraries-website-tools
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-maryland-college-park/refs/heads/main/openapi/university-of-maryland-college-park-libraries-website-tools-openapi.yml
auth_types: []
description: Authentication posture of the surfaces the University of Maryland actually operates itself. Every institution-operated library and repository read surface confirmed in this profile is open and keyless. The one exception is the campus Enterprise GIS, which publishes its service catalog without a credential and gates every service behind an ArcGIS token. Beyond that, the institution's authentication engineering is concentrated in its SAML identity provider, which authenticates people into vendor platforms rather than authorising API clients.
kind: authentication
layout: security
method: probed
name: University Of Maryland College Park Authentication
name_suffix: Authentication
oauth_flows: []
overview: University of Maryland College Park declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: University of Maryland College Park
provider_slug: university-of-maryland-college-park
scheme_count: 0
schemes: []
slug: university-of-maryland-college-park-authentication
source_filename: university-of-maryland-college-park-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: probed\nsource: live unauthenticated requests against each host, 2026-08-30\nx-operator: institution\nprovider: University of Maryland College Park\nproviderId: university-of-maryland-college-park\ndescription: >-\n  Authentication posture of the surfaces the University of Maryland actually operates itself.\n  Every institution-operated library and repository read surface confirmed in this profile is open\n  and keyless. The one exception is the campus Enterprise GIS, which publishes its service catalog\n  without a credential and gates every service behind an ArcGIS token. Beyond that, the institution's\n  authentication engineering is concentrated in its SAML identity provider, which authenticates\n  people into vendor platforms rather than authorising API clients.\nsurfaces:\n- name: UMD Libraries Website Tools API\n  baseURL: https://api.www.lib.umd.edu/api/libtools\n  scheme: none\n  api_key_required: false\n  evidence:\n    url: https://api.www.lib.umd.edu/api/libtools/mckeldin/availability\n\
  \    status: 200\n    note: Full JSON body returned with no Authorization header, no cookie and no key parameter.\n  declared_in_contract: false\n  note: >-\n    The upstream OpenAPI declares no securitySchemes and no security requirement. That matches\n    observed behaviour rather than omitting a requirement.\n- name: UMD Libraries Digital Collections OAI-PMH\n  baseURL: https://api.fcrepo.lib.umd.edu/oai/api\n  scheme: none\n  api_key_required: false\n  evidence:\n    url: https://api.fcrepo.lib.umd.edu/oai/api?verb=Identify\n    status: 200\n    note: OAI-PMH Identify returned unauthenticated.\n- name: UMD Libraries A/V Digital Collections OAI-PMH\n  baseURL: https://api.av.lib.umd.edu/oai/api\n  scheme: none\n  api_key_required: false\n  evidence:\n    url: https://api.av.lib.umd.edu/oai/api?verb=Identify\n    status: 200\n- name: UMD Archival Collections OAI-PMH\n  baseURL: https://archives-api.lib.umd.edu/oai\n  scheme: none\n  api_key_required: false\n  evidence:\n    url: https://archives-api.lib.umd.edu/oai?verb=Identify\n\
  \    status: 200\n- name: UMD Shibboleth Identity Provider\n  baseURL: https://shib.idm.umd.edu/idp/shibboleth\n  scheme: saml2\n  api_key_required: false\n  entityID: urn:mace:incommon:umd.edu\n  evidence:\n    url: https://shib.idm.umd.edu/idp/shibboleth\n    status: 200\n    note: >-\n      SAML 2.0 EntityDescriptor served unauthenticated, as the federation protocol requires.\n      This is a browser-SSO identity provider for people, not an OAuth/OIDC authorization\n      server for API clients; it issues no API tokens to third parties.\n  assurance:\n  - https://refeds.org/sirtfi\n  entity_categories:\n  - http://id.incommon.org/category/research-and-scholarship\n  - http://refeds.org/category/research-and-scholarship\n- name: UMD Enterprise GIS — ArcGIS REST Services\n  baseURL: https://gis.umd.edu/arcgis/rest/services\n  scheme: arcgis-token\n  api_key_required: true\n  self_service: false\n  token_endpoint: https://gis.umd.edu/portal/sharing/rest/generateToken\n  evidence:\n   \
  \ url: https://gis.umd.edu/arcgis/rest/info?f=json\n    status: 200\n    note: >-\n      authInfo.isTokenBasedSecurity true, tokenServicesUrl\n      https://gis.umd.edu/portal/sharing/rest/generateToken.\n  probes:\n  - url: https://gis.umd.edu/arcgis/rest/services?f=json\n    status: 200\n    note: Service catalog root enumerated 14 folders with no credential.\n  - url: https://gis.umd.edu/arcgis/rest/services/Navigation?f=json\n    status: 200\n    note: >-\n      HTTP 200 whose body is {\"error\":{\"code\":499,\"message\":\"Token Required\"}}. The status code is\n      not the answer here; the body is. Recorded so a reader does not score this folder as open.\n  - url: https://gis.umd.edu/portal/sharing/rest?f=json\n    status: 200\n    note: Portal version document readable unauthenticated.\n  declared_in_contract: true\n  note: >-\n    Tokens are issued by UMD's own ArcGIS Portal to accounts UMD provisions. There is no public\n    registration path, so this is a credentialed internal\
  \ surface with a public catalog, not a\n    developer programme.\ngaps:\n- No OAuth 2.0 or OpenID Connect authorization server is published for third-party API clients.\n- No developer key issuance, client registration, or self-service credentialing exists on any\n  institution-operated host found in this review.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-maryland-college-park/refs/heads/main/authentication/university-of-maryland-college-park-authentication.yml
summary_line: 0 schemes
tags:
- University
- Higher Education
- Education
- United States
- Maryland
- Public Research University
- Land Grant
- Big Ten
- Library
- Research Data
- Digital Collections
- Identity Federation
- OAI-PMH
- Open Data
- Geospatial
---
