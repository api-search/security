---
api_key_in: []
api_specs:
- filename: university-of-pittsburgh-project-tycho-api-openapi.yml
  format: yaml
  label: Project Tycho API
  slug: project-tycho
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-pittsburgh/refs/heads/main/openapi/university-of-pittsburgh-project-tycho-api-openapi.yml
auth_types:
- api_key
- none
- saml
description: ''
kind: authentication
layout: security
method: probed
name: University Of Pittsburgh Authentication
name_suffix: Authentication
oauth_flows: []
overview: University of Pittsburgh secures its APIs with api_key, none, and saml across 6 declared security schemes, as derived from its OpenAPI definitions.
provider_name: University of Pittsburgh
provider_slug: university-of-pittsburgh
scheme_count: 6
schemes:
- applies_to: https://www.tycho.pitt.edu/api
  defects:
  - An authentication failure is served with HTTP 200 and an HTML fragment. A client branching on response.ok, or a pipeline checking the status line, reads a rejected credential as a success.
  - The credential is a URL query parameter with no header alternative and no documented rotation, expiry or revocation path.
  description: 'Every Project Tycho API call carries the key in the query string as `apikey`. There is no header-based alternative, so the credential is written into server access logs, browser history, Referer headers and any intermediary cache that sees the URL. The key is also evaluated BEFORE routing: a request to a path that does not exist returns the same "Invalid API key" body as a real path, so an unauthenticated client cannot discover or verify the surface at all.'
  evidence:
    body: Invalid API key. Please see the <a href="/dataset/api">API Help</a> (https://www.tycho.pitt.edu/dataset/api) for more information.
    content_type: text/html
    status: 200
    url: https://www.tycho.pitt.edu/api/condition?apikey=INVALIDKEY
  location: query
  name: ProjectTychoApiKey
  operator: institution
  parameter: apikey
  registration: Free. Create an account at https://www.tycho.pitt.edu and read the key off the user Profile page. No approval step, plan tier or contract is documented.
  type: api_key
- applies_to: https://data.wprdc.org/api/3/action
  description: 'The Western Pennsylvania Regional Data Center''s CKAN Action API is readable with no credential. Probed keyless on 2026-08-30: package_search returned HTTP 200 with 24,782 bytes of JSON, status_show returned CKAN 2.11.6, package_list returned 13,372 bytes. CKAN''s write actions require an API token, but no public write path is offered here. Note that the portal presents a click-through Data Use Agreement to browsers which the API does not enforce.'
  evidence:
    content_type: application/json
    status: 200
    url: https://data.wprdc.org/api/3/action/package_search?rows=1
  name: WPRDCCkanPublicRead
  operator: institution
  type: none
- applies_to: https://anthro-age.pitt.edu/ojs/anthro-age/oai
  description: The University Library System's OAI-PMH 2.0 providers are open to anonymous harvesting. Identify, ListMetadataFormats and ListRecords all answered HTTP 200 with no credential on 2026-08-30 across four separate journal hosts.
  evidence:
    content_type: text/xml
    status: 200
    url: https://anthro-age.pitt.edu/ojs/anthro-age/oai?verb=Identify
  name: ULSOaiPmhPublicRead
  operator: institution
  type: none
- applies_to: https://anthro-age.pitt.edu/ojs/anthro-age/api/v1
  description: 'The PKP Open Journal Systems REST API is deployed alongside each OAI-PMH provider but is closed to the public: it answers HTTP 403 with {"error":"api.403.unauthorized"} to unauthenticated callers. OJS gates this API behind a per-user API token issued inside the journal, which is not obtainable by a member of the public. Recorded so the surface is not mistaken for an open one.'
  evidence:
    body: '{"error":"api.403.unauthorized","errorMessage":"You are not authorized to access the requested resource."}'
    content_type: application/json
    status: 403
    url: https://anthro-age.pitt.edu/ojs/anthro-age/api/v1/issues
  name: ULSOjsRestApiClosed
  operator: institution
  type: api_key
- applies_to: https://d-scholarship.pitt.edu/catalog/oai
  description: 'D-Scholarship@Pitt''s OAI-PMH provider is open to anonymous harvesting. Identify, ListMetadataFormats (oai_dc, oai_hyku) and ListRecords all answered HTTP 200 with no credential on 2026-08-30. Recorded with operator `tenant`: d-scholarship.pitt.edu CNAMEs to pittir.hykucommons.org and the provider is Hyku''s blacklight_oai_provider, so the content and the DOIs are Pitt''s but the endpoint and its access model are the platform''s. Note that the repository''s HTML surface at the same hostname returns HTTP 403 behind a Cloudflare challenge to the same client that the OAI path serves without complaint.'
  evidence:
    content_type: text/xml
    status: 200
    url: https://d-scholarship.pitt.edu/catalog/oai?verb=Identify
  name: DScholarshipOaiPmhPublicRead
  operator: tenant
  type: none
  vendor: Hyku Commons (Samvera Hyku)
- applies_to: https://passport.pitt.edu/idp/shibboleth
  description: Pitt Passport is the campus SAML 2.0 / Shibboleth identity provider. It authenticates people to relying service providers; it is not a data API and issues no credential a machine client can use to call one. Recorded because it is the most unambiguously institution-operated machine-readable surface the University of Pittsburgh publishes, and because it is what makes the `shibboleth` and `saml` conformance hits real.
  evidence:
    content_type: application/xml
    status: 200
    url: https://passport.pitt.edu/idp/shibboleth
  name: PittPassportShibboleth
  operator: institution
  type: saml
slug: university-of-pittsburgh-authentication
source_filename: university-of-pittsburgh-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "# authorship: API Evangelist. Not published by the University of Pittsburgh.\nx-method: derived\nx-authorship: >-\n  Written by API Evangelist from live probes of the University of Pittsburgh's own public\n  surfaces. Pitt publishes no equivalent document. The `method:` key below is the university\n  pipeline's provenance vocabulary (how we came to hold the facts); x-method above is the\n  authorship vocabulary the provenance manifest reads (who wrote the file).\ngenerated: '2026-08-30'\nmethod: probed\nsource: >-\n  Live probes on 2026-08-30 of every surface attributed to the University of Pittsburgh, plus the\n  published API reference at https://www.tycho.pitt.edu/dataset/api/ and\n  openapi/university-of-pittsburgh-project-tycho-api-openapi.yml.\nprovider: University of Pittsburgh\nproviderId: university-of-pittsburgh\nsummary:\n  types:\n  - api_key\n  - none\n  - saml\n  institution_operated_public_apis_requiring_no_auth: 2\n  institution_operated_public_apis_requiring_a_key:\
  \ 1\n  tenant_operated_public_apis_requiring_no_auth: 1\n  oauth_surfaces_operated_by_the_institution: 0\n  institution_wide_key_issuance: false\nschemes:\n- name: ProjectTychoApiKey\n  type: api_key\n  operator: institution\n  applies_to: https://www.tycho.pitt.edu/api\n  location: query\n  parameter: apikey\n  registration: >-\n    Free. Create an account at https://www.tycho.pitt.edu and read the key off the user Profile\n    page. No approval step, plan tier or contract is documented.\n  description: >-\n    Every Project Tycho API call carries the key in the query string as `apikey`. There is no\n    header-based alternative, so the credential is written into server access logs, browser\n    history, Referer headers and any intermediary cache that sees the URL. The key is also\n    evaluated BEFORE routing: a request to a path that does not exist returns the same \"Invalid\n    API key\" body as a real path, so an unauthenticated client cannot discover or verify the\n    surface at\
  \ all.\n  evidence:\n    url: https://www.tycho.pitt.edu/api/condition?apikey=INVALIDKEY\n    status: 200\n    content_type: text/html\n    body: 'Invalid API key. Please see the <a href=\"/dataset/api\">API Help</a> (https://www.tycho.pitt.edu/dataset/api) for more information.'\n  defects:\n  - >-\n    An authentication failure is served with HTTP 200 and an HTML fragment. A client branching on\n    response.ok, or a pipeline checking the status line, reads a rejected credential as a success.\n  - >-\n    The credential is a URL query parameter with no header alternative and no documented rotation,\n    expiry or revocation path.\n- name: WPRDCCkanPublicRead\n  type: none\n  operator: institution\n  applies_to: https://data.wprdc.org/api/3/action\n  description: >-\n    The Western Pennsylvania Regional Data Center's CKAN Action API is readable with no credential.\n    Probed keyless on 2026-08-30: package_search returned HTTP 200 with 24,782 bytes of JSON,\n    status_show returned\
  \ CKAN 2.11.6, package_list returned 13,372 bytes. CKAN's write actions\n    require an API token, but no public write path is offered here. Note that the portal presents a\n    click-through Data Use Agreement to browsers which the API does not enforce.\n  evidence:\n    url: https://data.wprdc.org/api/3/action/package_search?rows=1\n    status: 200\n    content_type: application/json\n- name: ULSOaiPmhPublicRead\n  type: none\n  operator: institution\n  applies_to: https://anthro-age.pitt.edu/ojs/anthro-age/oai\n  description: >-\n    The University Library System's OAI-PMH 2.0 providers are open to anonymous harvesting. Identify,\n    ListMetadataFormats and ListRecords all answered HTTP 200 with no credential on 2026-08-30\n    across four separate journal hosts.\n  evidence:\n    url: https://anthro-age.pitt.edu/ojs/anthro-age/oai?verb=Identify\n    status: 200\n    content_type: text/xml\n- name: ULSOjsRestApiClosed\n  type: api_key\n  operator: institution\n  applies_to: https://anthro-age.pitt.edu/ojs/anthro-age/api/v1\n\
  \  description: >-\n    The PKP Open Journal Systems REST API is deployed alongside each OAI-PMH provider but is closed\n    to the public: it answers HTTP 403 with {\"error\":\"api.403.unauthorized\"} to unauthenticated\n    callers. OJS gates this API behind a per-user API token issued inside the journal, which is not\n    obtainable by a member of the public. Recorded so the surface is not mistaken for an open one.\n  evidence:\n    url: https://anthro-age.pitt.edu/ojs/anthro-age/api/v1/issues\n    status: 403\n    content_type: application/json\n    body: '{\"error\":\"api.403.unauthorized\",\"errorMessage\":\"You are not authorized to access the requested resource.\"}'\n- name: DScholarshipOaiPmhPublicRead\n  type: none\n  operator: tenant\n  vendor: Hyku Commons (Samvera Hyku)\n  applies_to: https://d-scholarship.pitt.edu/catalog/oai\n  description: >-\n    D-Scholarship@Pitt's OAI-PMH provider is open to anonymous harvesting. Identify,\n    ListMetadataFormats (oai_dc, oai_hyku)\
  \ and ListRecords all answered HTTP 200 with no credential\n    on 2026-08-30. Recorded with operator `tenant`: d-scholarship.pitt.edu CNAMEs to\n    pittir.hykucommons.org and the provider is Hyku's blacklight_oai_provider, so the content and\n    the DOIs are Pitt's but the endpoint and its access model are the platform's. Note that the\n    repository's HTML surface at the same hostname returns HTTP 403 behind a Cloudflare challenge to\n    the same client that the OAI path serves without complaint.\n  evidence:\n    url: https://d-scholarship.pitt.edu/catalog/oai?verb=Identify\n    status: 200\n    content_type: text/xml\n- name: PittPassportShibboleth\n  type: saml\n  operator: institution\n  applies_to: https://passport.pitt.edu/idp/shibboleth\n  description: >-\n    Pitt Passport is the campus SAML 2.0 / Shibboleth identity provider. It authenticates people to\n    relying service providers; it is not a data API and issues no credential a machine client can\n    use to call one.\
  \ Recorded because it is the most unambiguously institution-operated\n    machine-readable surface the University of Pittsburgh publishes, and because it is what makes\n    the `shibboleth` and `saml` conformance hits real.\n  evidence:\n    url: https://passport.pitt.edu/idp/shibboleth\n    status: 200\n    content_type: application/xml\nnotes:\n- >-\n  The University of Pittsburgh operates no OAuth 2.0 authorization server, no API gateway, no\n  developer portal and no institution-wide key issuance. developer.pitt.edu and apis.pitt.edu do\n  not resolve; https://www.pitt.edu/apis.json and https://www.pitt.edu/llms.txt return 404. Each\n  surface above carries its own unrelated auth model because each was built by a different unit.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-pittsburgh/refs/heads/main/authentication/university-of-pittsburgh-authentication.yml
summary_line: api_key/none/saml · 6 schemes
tags:
- University
- Higher Education
- Education
- United States
- Public Research University
- Research Data
- Open Data
- Epidemiology
- Public Health
- Civic Data
- Scholarly Publishing
- Institutional Repository
- Library
- Identity Federation
- OAI-PMH
- Open Access
---
