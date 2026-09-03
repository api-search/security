---
api_key_in: []
api_specs:
- filename: ohio-state-university-mobile-content-api-openapi.yml
  format: yaml
  label: Ohio State Mobile Content API v2
  slug: mobile-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ohio-state-university/refs/heads/main/openapi/ohio-state-university-mobile-content-api-openapi.yml
auth_types: []
description: 'How each Ohio State surface in this profile is authenticated. Two very different postures sit side by side: a small number of genuinely open, unauthenticated read APIs, and an institution-wide SAML/Shibboleth Single Sign-On that gates everything else. There is no API key programme, no developer registration, and no published OAuth client onboarding for any Ohio State surface found in this run.'
kind: authentication
layout: security
method: probed
name: Ohio State University Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ohio State University declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Ohio State University
provider_slug: ohio-state-university
scheme_count: 0
schemes: []
slug: ohio-state-university-authentication
source_filename: ohio-state-university-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "---\naid: ohio-state-university\nname: Ohio State University authentication\ndescription: >-\n  How each Ohio State surface in this profile is authenticated. Two very different postures sit\n  side by side: a small number of genuinely open, unauthenticated read APIs, and an\n  institution-wide SAML/Shibboleth Single Sign-On that gates everything else. There is no API key\n  programme, no developer registration, and no published OAuth client onboarding for any Ohio\n  State surface found in this run.\ngenerated: '2026-09-01'\nmethod: probed\nsource:\n  - https://content.osu.edu/v2\n  - https://data.chrr.ohio-state.edu/api/3/action/status_show\n  - https://kb.osu.edu/server/api\n  - https://mdq.incommon.org/entities/urn%3Amace%3Aincommon%3Aosu.edu\nsurfaces:\n  - surface: Ohio State Mobile Content API v2\n    baseURL: https://content.osu.edu/v2\n    x-operator: institution\n    scheme: none\n    detail: >-\n      No authentication of any kind. Anonymous GET returns data; no key,\
  \ token, referer check or\n      rate-limit header was observed on 2026-09-01.\n    evidence:\n      - url: https://content.osu.edu/v2/classes/searchableTermsV2\n        status: 200\n  - surface: CHRR CKAN open data portal\n    baseURL: https://data.chrr.ohio-state.edu/api/3\n    x-operator: institution\n    scheme: none-for-read\n    detail: >-\n      CKAN 2.10.10 Action API. Read actions (status_show, package_list, package_show) are anonymous.\n      Write actions require a CKAN API token, and the deployment loads the saml2auth extension, so\n      account login is federated through Ohio State's own Shibboleth IdP rather than local CKAN\n      accounts.\n    evidence:\n      - url: https://data.chrr.ohio-state.edu/api/3/action/status_show\n        status: 200\n        note: 'extensions include saml2auth, chrrpermissions, doi, datastore, xloader.'\n  - surface: Knowledge Bank DSpace REST API\n    baseURL: https://kb.osu.edu/server/api\n    x-operator: tenant\n    scheme: none-for-read\n\
  \    detail: >-\n      DSpace 7.6 REST API. Public read of communities, collections, items and bitstreams is\n      anonymous. Authenticated operations use DSpace's own token flow, which is Atmire/DSpace\n      software, not an Ohio State authentication scheme.\n    evidence:\n      - url: https://kb.osu.edu/server/api\n        status: 200\n  - surface: Web Single Sign-On (Shibboleth IdP)\n    baseURL: https://webauth.service.ohio-state.edu/idp\n    x-operator: institution\n    scheme: saml2\n    detail: >-\n      SAML 2.0 via Shibboleth, published in InCommon under entityID urn:mace:incommon:osu.edu.\n      Redirect and POST SSO/SLO bindings plus SOAP ECP. Intended for registered campus and\n      cloud service owners integrating as SAML service providers, not for open public consumption\n      — there is no self-service SP registration surface.\n    evidence:\n      - url: https://mdq.incommon.org/entities/urn%3Amace%3Aincommon%3Aosu.edu\n        status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ohio-state-university/refs/heads/main/authentication/ohio-state-university-authentication.yml
summary_line: 0 schemes
tags:
- University
- Higher Education
- Education
- United States
- Public Research University
- Course Catalog
- Open Data
- Research Data
- Institutional Repository
- Library
- Identity Federation
- Open Access
---
