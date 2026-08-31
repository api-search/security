---
api_key_in: []
api_specs:
- filename: yale-search-api-openapi.yml
  format: yaml
  label: LUX Collections Discovery — Search API
  slug: yale-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yale/refs/heads/main/openapi/yale-search-api-openapi.yml
- filename: yale-documents-api-openapi.yml
  format: yaml
  label: LUX Collections Discovery — Documents API
  slug: yale-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yale/refs/heads/main/openapi/yale-documents-api-openapi.yml
- filename: yale-facets-api-openapi.yml
  format: yaml
  label: LUX Collections Discovery — Facets API
  slug: yale-facets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yale/refs/heads/main/openapi/yale-facets-api-openapi.yml
- filename: yale-related-api-openapi.yml
  format: yaml
  label: LUX Collections Discovery — Related API
  slug: yale-related-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yale/refs/heads/main/openapi/yale-related-api-openapi.yml
- filename: yale-configuration-api-openapi.yml
  format: yaml
  label: LUX Collections Discovery — Configuration API
  slug: yale-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yale/refs/heads/main/openapi/yale-configuration-api-openapi.yml
- filename: yale-federation-api-openapi.yml
  format: yaml
  label: Yale University Federation API
  slug: yale-federation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yale/refs/heads/main/openapi/yale-federation-api-openapi.yml
- filename: yale-iiif-api-openapi.yml
  format: yaml
  label: Yale University IIIF API
  slug: yale-iiif-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yale/refs/heads/main/openapi/yale-iiif-api-openapi.yml
- filename: yale-info-api-openapi.yml
  format: yaml
  label: Yale University Info API
  slug: yale-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yale/refs/heads/main/openapi/yale-info-api-openapi.yml
auth_types: []
description: 'How authentication works across Yale University''s machine-readable surfaces. Yale is unusual for its cohort in running a genuinely bifurcated estate: an entirely open cultural-heritage and research-data tier that needs no credential at all, and an entirely closed administrative tier that needs a Yale NetID before a key can even be requested.'
kind: authentication
layout: security
method: probed
name: Yale Authentication
name_suffix: Authentication
oauth_flows: []
overview: Yale University declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Yale University
provider_slug: yale
scheme_count: 0
schemes: []
slug: yale-authentication
source_filename: yale-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-19'\nmethod: probed\nsource: >-\n  Live probes on 2026-08-19 of gw.its.yale.edu, developers.yale.edu, lux.collections.yale.edu,\n  dataverse.yale.edu, collections.library.yale.edu and auth.yale.edu, plus the published access\n  policy at https://developers.yale.edu/how-info/how-do-i-get-access-apis\ndescription: >-\n  How authentication works across Yale University's machine-readable surfaces. Yale is unusual for\n  its cohort in running a genuinely bifurcated estate: an entirely open cultural-heritage and\n  research-data tier that needs no credential at all, and an entirely closed administrative tier\n  that needs a Yale NetID before a key can even be requested.\nauthentication:\n- surface: LUX Collections Discovery API\n  base_url: https://lux.collections.yale.edu\n  x-operator: institution\n  scheme: none\n  public: true\n  evidence:\n    url: https://lux.collections.yale.edu/api/search-estimate/item?q=%7B%22text%22%3A%22gold%22%7D\n    status: 200\n\
  \  note: >-\n    Public read endpoints are unauthenticated and returned 53,387 matching objects on an anonymous\n    call. Write and admin endpoints on the MarkLogic backend are not publicly exposed.\n- surface: Yale Dataverse Repository API\n  base_url: https://dataverse.yale.edu\n  x-operator: institution\n  scheme: none\n  public: true\n  privileged_scheme: api_key\n  privileged_mechanism: X-Dataverse-key header\n  evidence:\n    url: https://dataverse.yale.edu/api/search?q=yale\n    status: 200\n  note: >-\n    Published content reads anonymously. Deposit, draft access and administrative calls require a\n    Dataverse API token issued after Yale NetID login; no token was obtained or used.\n- surface: Yale University Library Digital Collections IIIF\n  base_url: https://collections.library.yale.edu\n  x-operator: institution\n  scheme: none\n  public: true\n  evidence:\n    url: https://collections.library.yale.edu/manifests/2055095\n    status: 200\n  note: >-\n    IIIF manifests serve\
  \ unauthenticated. The Blacklight JSON surface at /catalog.json and\n    /catalog/{oid}.json returned an empty HTTP 202 to every automated request tried, including\n    with a browser User-Agent and Accept: application/json — an edge bot challenge, not a 401 and\n    not a 404. Recorded as gated at the edge rather than as an authentication scheme.\n- surface: Yale Identity Federation metadata\n  base_url: https://auth.yale.edu\n  x-operator: institution\n  scheme: none\n  public: true\n  evidence:\n    url: https://auth.yale.edu/idp/shibboleth\n    status: 200\n  note: >-\n    The metadata document itself is deliberately public — that is what federation metadata is for.\n    The IdP it describes authenticates via SAML 2.0 / Shibboleth against Yale NetID, and Yale also\n    fronts legacy applications with CAS at https://secure.its.yale.edu/cas/login (200 verified).\n- surface: Yale Portal APIs (Buildings, Courses, Course Subjects, GatewayServiceMetrics)\n  base_url: https://gw.its.yale.edu\n\
  \  x-operator: institution\n  scheme: api_key\n  public: false\n  gate: Yale NetID required to reach the developer portal and register an application\n  evidence:\n  - url: https://gw.its.yale.edu/soa-gateway/courses/webservice/v3/index\n    status: 400\n    body: 'Invalid API Key'\n  - url: https://developers.yale.edu/how-info/how-do-i-get-access-apis\n    status: 200\n  note: >-\n    The gateway is LIVE and answering — it rejected an anonymous call with a specific\n    \"Invalid API Key\" body rather than timing out. Yale's own portal describes these as INTERNAL\n    APIs. This corrects an earlier profile of this repository that described the Courses Web\n    Service as returning \"public information\": the payload may be public information, but the\n    surface is not publicly accessible.\n- surface: Yale Enterprise (SOA) Services (People Hub, COA, Workday Supervisory Orgs)\n  base_url: https://gw.its.yale.edu\n  x-operator: institution\n  scheme: basic\n  public: false\n  gate: Service\
  \ account, provisioned under named data-governance policies\n  evidence:\n    url: https://developers.yale.edu/api-documentation/enterprise-soa-services\n    status: 200\n  note: >-\n    Eleven services delivered by Yale's Integration Competency Center. Yale's own page calls them\n    \"Private APIs that use basic authentication via a service account\" with \"specific request and\n    data governance policies\". Documented publicly, callable only internally.\n- surface: EliScholar OAI-PMH\n  base_url: https://elischolar.library.yale.edu\n  x-operator: tenant\n  scheme: none\n  public: true\n  evidence:\n    url: https://elischolar.library.yale.edu/do/oai/?verb=Identify\n    status: 200\n  note: Harvesting is open. The endpoint is operated by Elsevier's bepress Digital Commons.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yale/refs/heads/main/authentication/yale-authentication.yml
summary_line: 0 schemes
tags:
- University
- Higher Education
- Education
- United States
- Ivy League
- Research
- Research Data
- Research Repository
- Identity Federation
- Library
- Cultural Heritage
- Linked Data
- IIIF
- Course Catalog
---
