---
api_key_in: []
api_specs:
- filename: university-of-oxford-iiif-api-openapi.yml
  format: yaml
  label: University of Oxford IIIF API
  slug: university-of-oxford-iiif-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-oxford/refs/heads/main/openapi/university-of-oxford-iiif-api-openapi.yml
- filename: university-of-oxford-oai-pmh-api-openapi.yml
  format: yaml
  label: University of Oxford OAI PMH API
  slug: university-of-oxford-oai-pmh-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-oxford/refs/heads/main/openapi/university-of-oxford-oai-pmh-api-openapi.yml
- filename: university-of-oxford-repository-api-openapi.yml
  format: yaml
  label: University of Oxford Repository API
  slug: university-of-oxford-repository-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-oxford/refs/heads/main/openapi/university-of-oxford-repository-api-openapi.yml
- filename: university-of-oxford-textarchive-api-openapi.yml
  format: yaml
  label: University of Oxford Text Archive API
  slug: university-of-oxford-textarchive-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-oxford/refs/heads/main/openapi/university-of-oxford-textarchive-api-openapi.yml
auth_types: []
description: 'Every institution-operated API surface found at Oxford is unauthenticated and read-only. Authentication at Oxford exists, and is substantial, but it sits on the identity-federation side of the house rather than in front of any public API: there is no API key, no OAuth client registration, no developer account and no token endpoint anywhere in the estate.'
kind: authentication
layout: security
method: probed
name: University Of Oxford Authentication
name_suffix: Authentication
oauth_flows: []
overview: University of Oxford declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: University of Oxford
provider_slug: university-of-oxford
scheme_count: 0
schemes: []
slug: university-of-oxford-authentication
source_filename: university-of-oxford-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "name: University of Oxford — authentication posture\ndescription: >-\n  Every institution-operated API surface found at Oxford is unauthenticated and read-only.\n  Authentication at Oxford exists, and is substantial, but it sits on the identity-federation\n  side of the house rather than in front of any public API: there is no API key, no OAuth\n  client registration, no developer account and no token endpoint anywhere in the estate.\ngenerated: '2026-08-19'\nmethod: probed\nsource: live unauthenticated HTTP probes of every surface listed in apis.yml\nsurfaces:\n  - api: ORA OAI-PMH\n    url: https://ora.ox.ac.uk/oai2\n    x-operator: institution\n    scheme: none\n    detail: >-\n      Fully open to unauthenticated harvesting. Oxford states in its own guidance that large or\n      bulk harvesters should contact the service first — a social control, not a technical one,\n      and it is not enforced by credentials.\n  - api: ORA search / object JSON\n    url: https://ora.ox.ac.uk/objects.json\n\
  \    x-operator: institution\n    scheme: none\n    detail: >-\n      No authentication. Cloudflare fronts the host and issues a managed challenge on some\n      paths (a 403 with cf-mitigated: challenge on /objects/opensearch.xml), which is bot\n      mitigation rather than an access-control scheme.\n  - api: Digital Bodleian IIIF\n    url: https://iiif.bodleian.ox.ac.uk\n    x-operator: institution\n    scheme: none\n    detail: >-\n      Open. IIIF defines an Authentication API; this deployment does not use it, and no auth\n      services are advertised on the info.json or manifest documents.\n  - api: Oxford Text Archive OAI-PMH\n    url: https://ota.bodleian.ox.ac.uk/repository/oai/request\n    x-operator: institution\n    scheme: none\n  - api: Continuing Education WordPress REST\n    url: https://lifelong-learning.ox.ac.uk/wp-json/\n    x-operator: institution\n    scheme: none\n    detail: >-\n      Read paths are anonymous. WordPress write endpoints exist in the route table but\
  \ require\n      cookie or application-password auth that is not offered to the public.\nfederated-identity:\n  detail: >-\n    Where Oxford does authenticate, it does so through SAML 2.0 rather than through anything an\n    API client can obtain. The University operates a Shibboleth Identity Provider registered in\n    the UK Access Management Federation and eduGAIN as\n    https://registry.shibboleth.ox.ac.uk/idp, plus two test IdPs, and 35 registered service\n    providers across central IT, departments and colleges. That is a real, machine-readable,\n    institution-operated authentication surface — it is simply not an API authorization scheme,\n    and it is recorded here so the absence above is not misread as an absence of identity\n    infrastructure.\n  evidence:\n    - url: https://idp.shibboleth.ox.ac.uk/idp/shibboleth\n      status: 200\n    - url: https://technical.edugain.org/api.php?action=list_entities&format=json\n      status: 200\ngaps:\n  - No developer account, API\
  \ key issuance or client registration anywhere in the estate.\n  - No OAuth 2.0 or OpenID Connect endpoint on any institution-operated host.\n  - >-\n    No documented authentication for the ORA JSON endpoints because those endpoints are not\n    documented at all — see openapi/university-of-oxford-ora-search-openapi.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-oxford/refs/heads/main/authentication/university-of-oxford-authentication.yml
summary_line: 0 schemes
tags:
- University
- Higher Education
- Education
- Research
- United Kingdom
- Russell Group
- Research Repository
- Library
- Digital Collections
- IIIF
- OAI-PMH
- Identity Federation
- Open Access
- Research Computing
---
