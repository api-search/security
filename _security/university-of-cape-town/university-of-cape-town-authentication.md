---
api_key_in: []
api_specs:
- filename: university-of-cape-town-catalog-api-openapi.yml
  format: yaml
  label: DataFirst Microdata Catalog API (NADA)
  slug: datafirst-nada
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-cape-town/refs/heads/main/openapi/university-of-cape-town-catalog-api-openapi.yml
auth_types: []
description: How each University of Cape Town surface authenticates callers. Every row was established by an actual request, not by reading documentation.
kind: authentication
layout: security
method: probed
name: University Of Cape Town Authentication
name_suffix: Authentication
oauth_flows: []
overview: University of Cape Town declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: University of Cape Town
provider_slug: university-of-cape-town
scheme_count: 0
schemes: []
slug: university-of-cape-town-authentication
source_filename: university-of-cape-town-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: probed\nsource: >-\n  Live unauthenticated requests run 2026-08-30 against\n  www.datafirst.uct.ac.za, open.uct.ac.za and metadata.safire.ac.za.\nx-operator: institution\ndescription: >-\n  How each University of Cape Town surface authenticates callers. Every row was\n  established by an actual request, not by reading documentation.\nsurfaces:\n  - name: DataFirst Microdata Catalog API (NADA)\n    x-operator: institution\n    base_url: https://www.datafirst.uct.ac.za/dataportal/index.php/api\n    scheme: none\n    public_read: true\n    api_key_required: false\n    signup_required: false\n    evidence:\n      - url: https://www.datafirst.uct.ac.za/dataportal/index.php/api/catalog?limit=2\n        status: 200\n        note: >-\n          Returned 582 studies with no credential of any kind, no cookie and no\n          Authorization header.\n    notes: >-\n      Catalog METADATA is fully open. The underlying microdata is not: studies\n      carry\
  \ form_model / data_access_type values such as `licensed`, and\n      downloading those files requires a DataFirst account and an approved\n      access request through the web portal, which has no API. Some collection\n      endpoints are closed outright — GET /collections returns\n      {\"status\":\"ACCESS-DENIED\"} with HTTP 400.\n  - name: OpenUCT repository — OAI-PMH\n    x-operator: institution\n    base_url: https://open.uct.ac.za/server/oai/request\n    scheme: none\n    public_read: true\n    evidence:\n      - url: https://open.uct.ac.za/server/oai/request?verb=Identify\n        status: 200\n  - name: OpenUCT repository — DSpace REST API\n    x-operator: institution\n    base_url: https://open.uct.ac.za/server/api\n    scheme: none for public read; DSpace session token for anything else\n    public_read: true\n    evidence:\n      - url: https://open.uct.ac.za/server/api\n        status: 200\n        content_type: application/hal+json\n        note: 'dspaceVersion \"DSpace 7.4\"\
  ; advertises an authn endpoint at /server/api/authn'\n      - url: https://open.uct.ac.za/server/api/discover/search/objects?size=1\n        status: 200\n        note: discovery search returns results anonymously\n    notes: >-\n      The authentication contract here is DSpace's, not UCT-authored — UCT\n      operates the deployment. Write and workflow endpoints require a DSpace\n      login backed by UCT credentials.\n  - name: UCT identity provider (SAML 2.0)\n    x-operator: institution\n    entity_id: https://srvslsfed001.uct.ac.za/simplesaml/saml2/idp/metadata.php\n    scheme: SAML 2.0 web browser SSO\n    public_read: false\n    single_sign_on: https://idp.uct.ac.za/simplesaml/module.php/saml/idp/singleSignOnService\n    single_logout: https://idp.uct.ac.za/simplesaml/module.php/saml/idp/singleLogout\n    name_id_format: urn:oasis:names:tc:SAML:2.0:nameid-format:transient\n    evidence:\n      - url: https://metadata.safire.ac.za/safire-prod-idp.xml\n        status: 200\n    notes:\
  \ >-\n      This is how humans and services authenticate INTO UCT systems. It is a\n      federation surface, not a REST API — there is no token endpoint an agent\n      can call.\n  - name: ZivaHub open data\n    x-operator: tenant\n    base_url: https://api.figshare.com/v2\n    scheme: none for public read; Figshare OAuth 2.0 / personal token for writes\n    evidence:\n      - url: https://zivahub.uct.ac.za/\n        status: 202\n        note: >-\n          Empty 202 from the Figshare edge — a bot challenge, not a dead host.\n          zivahub.uct.ac.za CNAMEs to figshare.com.\n    notes: >-\n      The authentication contract belongs to Figshare and is scored against\n      Figshare's own repo, not UCT's.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-cape-town/refs/heads/main/authentication/university-of-cape-town-authentication.yml
summary_line: 0 schemes
tags:
- University
- Higher Education
- Education
- Public Research University
- South Africa
- Africa
- Research Data
- Open Data
- Institutional Repository
- OAI-PMH
- Identity Federation
- Microdata
- Research Computing
---
