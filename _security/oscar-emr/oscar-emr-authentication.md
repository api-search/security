---
api_key_in: []
auth_types:
- oauth1a
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Oscar Emr Authentication
name_suffix: Authentication
oauth_flows: []
overview: OSCAR EMR secures its APIs with oauth1a and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: OSCAR EMR
provider_slug: oscar-emr
scheme_count: 2
schemes:
- endpoints:
    authorize: /ws/oauth/authorize?oauth_token=<request_token>
    initiate: /ws/oauth/initiate
    token: /ws/oauth/token
  flow: three-legged
  name: OAuth 1.0a
  note: Host and web context are deployment-specific (documented example http://localhost:8080/oscar_15/ws/oauth/...); there is no single public authorization server.
  registration: Applications are registered in the OSCAR Administration interface under Integration -> REST Clients (application name + valid base URI); registration issues a Client Key and Client Secret.
  spec: https://oauth.net/core/1.0a/
  surface: REST web services (/ws/services)
  transport: Authorization header on each REST call; HTTP 401 challenges when authorization is required
  type: oauth1a
- name: SMART on FHIR / SMART App Launch
  note: OSCAR Pro exposes a SMART on FHIR HL7 API for third-party app integration (contextual launch, FHIR eReferral). SMART App Launch is OAuth 2.0 based. Endpoints are per-deployment and gated to partners via the apps.health marketplace; no public authorization-server metadata is published.
  surface: FHIR HL7 API (OSCAR Pro distribution by WELL EMR Group)
  type: oauth2
slug: oscar-emr-authentication
source_filename: oscar-emr-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: searched\nsource: https://oscaremr.atlassian.net/wiki/spaces/OS/pages/79855638/Connecting+to+OSCAR's+REST+API\ndocs: https://oscaremr.atlassian.net/wiki/spaces/OS/pages/79855638/Connecting+to+OSCAR's+REST+API\nnote: >-\n  OSCAR publishes no OpenAPI/Swagger security schemes (runtime docs are RAML for JAX-RS), so this\n  profile is captured from the developer wiki and the JAX-RS source rather than derived from a spec.\n  The REST web-services layer (/ws/services) is protected by 3-legged OAuth 1.0a; the SMART on FHIR\n  surface exposed by the commercial OSCAR Pro distribution uses OAuth 2.0 / SMART App Launch.\nsummary:\n  types:\n  - oauth1a\n  - oauth2\n  oauth1a_flow: 3-legged (request token -> user authorize -> access token)\n  oauth2_context: SMART on FHIR / SMART App Launch (OSCAR Pro)\nschemes:\n- name: OAuth 1.0a\n  type: oauth1a\n  spec: https://oauth.net/core/1.0a/\n  surface: REST web services (/ws/services)\n  flow: three-legged\n\
  \  registration: >-\n    Applications are registered in the OSCAR Administration interface under Integration -> REST\n    Clients (application name + valid base URI); registration issues a Client Key and Client Secret.\n  endpoints:\n    initiate: /ws/oauth/initiate\n    authorize: /ws/oauth/authorize?oauth_token=<request_token>\n    token: /ws/oauth/token\n  transport: Authorization header on each REST call; HTTP 401 challenges when authorization is required\n  note: >-\n    Host and web context are deployment-specific (documented example\n    http://localhost:8080/oscar_15/ws/oauth/...); there is no single public authorization server.\n- name: SMART on FHIR / SMART App Launch\n  type: oauth2\n  surface: FHIR HL7 API (OSCAR Pro distribution by WELL EMR Group)\n  note: >-\n    OSCAR Pro exposes a SMART on FHIR HL7 API for third-party app integration (contextual launch,\n    FHIR eReferral). SMART App Launch is OAuth 2.0 based. Endpoints are per-deployment and gated to\n    partners via\
  \ the apps.health marketplace; no public authorization-server metadata is published.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oscar-emr/refs/heads/main/authentication/oscar-emr-authentication.yml
summary_line: oauth1a/oauth2 · 2 schemes
tags:
- Healthcare
- Canada
- EHR
- EMR
- Primary Care
- Open-Source
- FHIR
- HL7
- Interoperability
- SMART on FHIR
- Authentication
---
