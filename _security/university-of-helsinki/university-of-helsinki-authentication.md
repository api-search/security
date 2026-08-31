---
api_key_in:
- header
api_specs:
- filename: university-of-helsinki-hy-organisation-api-openapi.yml
  format: yaml
  label: HY Organisation API
  slug: hy-organisation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-helsinki/refs/heads/main/openapi/university-of-helsinki-hy-organisation-api-openapi.yml
- filename: university-of-helsinki-contact-search-api-openapi.yml
  format: yaml
  label: Contact Search API
  slug: contact-search
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-helsinki/refs/heads/main/openapi/university-of-helsinki-contact-search-api-openapi.yml
- filename: university-of-helsinki-course-pages-cms-openapi.yml
  format: yaml
  label: Course pages CMS
  slug: course-pages-cms
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-helsinki/refs/heads/main/openapi/university-of-helsinki-course-pages-cms-openapi.yml
- filename: university-of-helsinki-helsinki-fi-content-openapi.yml
  format: yaml
  label: Helsinki.fi content
  slug: helsinki-fi-content
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-helsinki/refs/heads/main/openapi/university-of-helsinki-helsinki-fi-content-openapi.yml
- filename: university-of-helsinki-hy-building-api-openapi.yml
  format: yaml
  label: HY Building API
  slug: hy-building
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-helsinki/refs/heads/main/openapi/university-of-helsinki-hy-building-api-openapi.yml
- filename: university-of-helsinki-serviceapi-openapi.yml
  format: yaml
  label: ServiceAPI
  slug: serviceapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-helsinki/refs/heads/main/openapi/university-of-helsinki-serviceapi-openapi.yml
- filename: university-of-helsinki-employeeinformationapi-openapi.yml
  format: yaml
  label: EmployeeInformationAPI
  slug: employeeinformation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-helsinki/refs/heads/main/openapi/university-of-helsinki-employeeinformationapi-openapi.yml
- filename: university-of-helsinki-persongroup-openapi.yml
  format: yaml
  label: PersonGroup
  slug: persongroup
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-helsinki/refs/heads/main/openapi/university-of-helsinki-persongroup-openapi.yml
- filename: university-of-helsinki-general-efecte-api-openapi.yml
  format: yaml
  label: General Efecte API
  slug: general-efecte
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-helsinki/refs/heads/main/openapi/university-of-helsinki-general-efecte-api-openapi.yml
- filename: university-of-helsinki-network-registry-api-openapi.yml
  format: yaml
  label: Network registry API
  slug: network-registry
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-helsinki/refs/heads/main/openapi/university-of-helsinki-network-registry-api-openapi.yml
- filename: university-of-helsinki-sovellussalkku-api-openapi.yml
  format: yaml
  label: Sovellussalkku API
  slug: sovellussalkku
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-helsinki/refs/heads/main/openapi/university-of-helsinki-sovellussalkku-api-openapi.yml
- filename: university-of-helsinki-dawa-sync-api-openapi.yml
  format: yaml
  label: Dawa Sync API
  slug: dawa-sync
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-helsinki/refs/heads/main/openapi/university-of-helsinki-dawa-sync-api-openapi.yml
- filename: university-of-helsinki-finbif-laji-openapi.yml
  format: yaml
  label: FinBIF Laji API (Finnish Biodiversity Information Facility)
  slug: finbif-laji
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-helsinki/refs/heads/main/openapi/university-of-helsinki-finbif-laji-openapi.yml
auth_types:
- apiKey
- http-bearer
- oauth2
description: ''
kind: authentication
layout: security
method: probed
name: University Of Helsinki Authentication
name_suffix: Authentication
oauth_flows: []
overview: University of Helsinki secures its APIs with apiKey, http-bearer, and oauth2 across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: University of Helsinki
provider_slug: university-of-helsinki
scheme_count: 5
schemes:
- in: header
  name: X-Api-Key
  note: The dominant scheme. Two specs case the header differently in the document (`X-API-Key` in the network registry spec, `X-Api-Key` everywhere else); HTTP header names are case-insensitive so both work, but the inconsistency is the provider's.
  parameter: X-Api-Key
  type: apiKey
  used_by:
  - openapi/university-of-helsinki-employeeinformationapi-openapi.yml
  - openapi/university-of-helsinki-general-efecte-api-openapi.yml
  - openapi/university-of-helsinki-hy-building-api-openapi.yml
  - openapi/university-of-helsinki-hy-organisation-api-openapi.yml
  - openapi/university-of-helsinki-persongroup-openapi.yml
  - openapi/university-of-helsinki-serviceapi-openapi.yml
  - openapi/university-of-helsinki-helsinki-fi-content-openapi.yml
  - openapi/university-of-helsinki-network-registry-api-openapi.yml
- flows: []
  name: oauth2
  note: Declared with NO flows, no authorizationUrl, no tokenUrl and no scopes, and its description links to `https://developers.getbase.com/docs/rest/articles/oauth2/requests` — an unrelated third-party CRM vendor. This is Drupal Simple OAuth boilerplate that shipped into the published spec unedited. Recorded because it is what the provider publishes, not because it is usable.
  type: oauth2
  used_by:
  - openapi/university-of-helsinki-course-pages-cms-openapi.yml
- in: header
  name: X-CSRF-Token
  note: Drupal JSON:API CSRF token, required on writes to the course-pages CMS.
  parameter: X-CSRF-Token
  token_url: https://cms.studies.helsinki.fi/user/token
  type: apiKey
  used_by:
  - openapi/university-of-helsinki-course-pages-cms-openapi.yml
- bearer_format: JWT
  name: Access token
  note: 'FinBIF (api.laji.fi) is the exception to the gateway story — it is operated by the Finnish Museum of Natural History, a University of Helsinki institute, on its own host with its own auth. Self-service: POST an email address to /api-user and the access token is mailed back. This is the only genuinely public, no-affiliation-required credential in the estate.'
  scheme: bearer
  type: http
  used_by:
  - openapi/university-of-helsinki-finbif-laji-openapi.yml
- in: header
  name: Person-Token
  note: Second FinBIF credential, identifying an end user rather than the calling application.
  parameter: Person-Token
  type: apiKey
  used_by:
  - openapi/university-of-helsinki-finbif-laji-openapi.yml
slug: university-of-helsinki-authentication
source_filename: university-of-helsinki-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: probed\nsource: https://api.helsinki.fi/portal/environments/DEFAULT/configuration\ndocs: https://api.helsinki.fi/portal/\nx-operator: institution\nsummary:\n  types:\n  - apiKey\n  - http-bearer\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows: []\n  note: >-\n    The University of Helsinki fronts its own APIs with a self-hosted Gravitee API Management\n    gateway. The gateway is https://gw.api.helsinki.fi and the developer portal is\n    https://api.helsinki.fi/portal/. The portal's own configuration endpoint states the\n    credential header (`X-Api-Key`) and which plan security types the environment enables:\n    apikey, oauth2 and jwt are enabled, sharedApiKey and keyless are DISABLED. Keyless being\n    off is the single most important access fact here — no University of Helsinki gateway API\n    is callable anonymously, whatever the OpenAPI shows.\ngateway:\n  product: Gravitee API Management\n  entrypoint: https://gw.api.helsinki.fi\n\
  \  portal: https://api.helsinki.fi/portal/\n  api_key_header: X-Api-Key\n  plan_security:\n    apikey: true\n    oauth2: true\n    jwt: true\n    sharedApiKey: false\n    keyless: false\n  evidence: >-\n    GET https://api.helsinki.fi/portal/environments/DEFAULT/configuration -> 200 application/json,\n    `portal.entrypoint`, `portal.apikeyHeader`, `plan.security.*` read verbatim.\nonboarding:\n  self_service_for_public: false\n  local_login_enabled: false\n  user_creation_enabled: false\n  application_creation_enabled: true\n  steps:\n  - Sign in to api.helsinki.fi with the HY Login Service (institutional SSO).\n  - Create an application from the Applications menu.\n  - Subscribe the application to an API in the API Gallery and choose a plan.\n  - A key is issued against that subscription.\n  note: >-\n    `authentication.localLogin.enabled` is false and `portal.userCreation.enabled` is false, so\n    there is no way for someone without a University of Helsinki (or Haka-federated) identity\
  \ to\n    register. The catalogue, the documentation and every OpenAPI are readable without signing in;\n    obtaining a credential is not. This is affiliation-gated, not paywalled.\n  evidence:\n  - url: https://api.helsinki.fi/portal/environments/DEFAULT/pages/0ff46388-9523-430b-b463-889523630b2f/content\n    status: 200\n    note: '\"How to get started\" portal page, four-step subscription flow, links the HY Developers wiki.'\n  - url: https://wiki.helsinki.fi/X/me05mC\n    status: 401\n    note: >-\n      HY Developers wiki, referenced by the portal as the fuller (mostly Finnish) documentation.\n      Auth-gated, so it is NOT emitted as a pointer in apis.yml — a 401 pointer reads as a claim\n      and grades as dead.\nschemes:\n- name: X-Api-Key\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  used_by:\n  - openapi/university-of-helsinki-employeeinformationapi-openapi.yml\n  - openapi/university-of-helsinki-general-efecte-api-openapi.yml\n  - openapi/university-of-helsinki-hy-building-api-openapi.yml\n\
  \  - openapi/university-of-helsinki-hy-organisation-api-openapi.yml\n  - openapi/university-of-helsinki-persongroup-openapi.yml\n  - openapi/university-of-helsinki-serviceapi-openapi.yml\n  - openapi/university-of-helsinki-helsinki-fi-content-openapi.yml\n  - openapi/university-of-helsinki-network-registry-api-openapi.yml\n  note: >-\n    The dominant scheme. Two specs case the header differently in the document (`X-API-Key` in\n    the network registry spec, `X-Api-Key` everywhere else); HTTP header names are\n    case-insensitive so both work, but the inconsistency is the provider's.\n- name: oauth2\n  type: oauth2\n  flows: []\n  used_by:\n  - openapi/university-of-helsinki-course-pages-cms-openapi.yml\n  note: >-\n    Declared with NO flows, no authorizationUrl, no tokenUrl and no scopes, and its description\n    links to `https://developers.getbase.com/docs/rest/articles/oauth2/requests` — an unrelated\n    third-party CRM vendor. This is Drupal Simple OAuth boilerplate that shipped\
  \ into the\n    published spec unedited. Recorded because it is what the provider publishes, not because it\n    is usable.\n- name: X-CSRF-Token\n  type: apiKey\n  in: header\n  parameter: X-CSRF-Token\n  token_url: https://cms.studies.helsinki.fi/user/token\n  used_by:\n  - openapi/university-of-helsinki-course-pages-cms-openapi.yml\n  note: Drupal JSON:API CSRF token, required on writes to the course-pages CMS.\n- name: Access token\n  type: http\n  scheme: bearer\n  bearer_format: JWT\n  used_by:\n  - openapi/university-of-helsinki-finbif-laji-openapi.yml\n  note: >-\n    FinBIF (api.laji.fi) is the exception to the gateway story — it is operated by the Finnish\n    Museum of Natural History, a University of Helsinki institute, on its own host with its own\n    auth. Self-service: POST an email address to /api-user and the access token is mailed back.\n    This is the only genuinely public, no-affiliation-required credential in the estate.\n- name: Person-Token\n  type: apiKey\n  in:\
  \ header\n  parameter: Person-Token\n  used_by:\n  - openapi/university-of-helsinki-finbif-laji-openapi.yml\n  note: Second FinBIF credential, identifying an end user rather than the calling application.\nnon_gateway_surfaces:\n- surface: Helda DSpace REST API\n  auth: none for read; DSpace `/server/api/authn` for write\n  evidence: 'GET https://helda.helsinki.fi/server/api -> 200 application/hal+json, authn link present.'\n- surface: HY Data Catalogue DSpace REST API\n  auth: none for read; DSpace `/server/api/authn` for write\n  evidence: 'GET https://datakatalogi.helsinki.fi/server/api -> 200 application/hal+json, DSpace 9.0.'\n- surface: OAI-PMH (Helda, HY Data Catalogue, Editori journals)\n  auth: none — anonymous harvesting by protocol design\n- surface: Sisu / Kori\n  auth: none observed on read paths, but the surface is a Funidata product, not a UH contract\n  evidence: >-\n    GET https://sisu.helsinki.fi/kori/api/module-search -> 400 application/json\n    {\"message\":\"AT_LEAST_ONE_SEARCH_PARAM_REQUIRED\"\
  } — answered without a credential.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-helsinki/refs/heads/main/authentication/university-of-helsinki-authentication.yml
summary_line: apiKey/http-bearer/oauth2 · 5 schemes
tags:
- Education
- Higher Education
- University
- Finland
- Nordic
- Research
- Open Data
- Research Data
- Institutional Repository
- OAI-PMH
- Identity Federation
- API Gateway
- Course Catalog
- Library
- Biodiversity
---
