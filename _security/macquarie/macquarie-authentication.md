---
api_key_in: []
api_specs:
- filename: macquarie-research-portal-oai-pmh-openapi.yml
  format: yaml
  label: Macquarie University Research Portal OAI-PMH
  slug: research-portal-oai-pmh
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/macquarie/refs/heads/main/openapi/macquarie-research-portal-oai-pmh-openapi.yml
auth_types:
- none
description: ''
kind: authentication
layout: security
method: probed
name: Macquarie Authentication
name_suffix: Authentication
oauth_flows: []
overview: Macquarie University secures its APIs with none across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Macquarie University
provider_slug: macquarie
scheme_count: 1
schemes:
- description: Anonymous HTTPS GET. Confirmed by executing all six OAI-PMH verbs with no credential.
  evidence:
  - status: 200
    url: https://research-management.mq.edu.au/ws/oai?verb=Identify
  - status: 200
    url: https://research-management.mq.edu.au/ws/oai?verb=ListMetadataFormats
  - status: 200
    url: https://research-management.mq.edu.au/ws/oai?verb=ListIdentifiers&metadataPrefix=oai_dc&set=publications:all
  name: none
  sources:
  - openapi/macquarie-research-portal-oai-pmh-openapi.yml
  type: none
slug: macquarie-authentication
source_filename: macquarie-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "# authorship: derived by API Evangelist from live, unauthenticated probes of the endpoint\n# on 2026-08-30. Macquarie University publishes no such document; this is OURS, not theirs.\n# x-method: derived\n# x-source-url: https://research-management.mq.edu.au/ws/oai\ngenerated: '2026-08-30'\nmethod: probed\nsource: https://research-management.mq.edu.au/ws/oai\nx-operator: institution\nsummary:\n  types:\n  - none\n  note: >-\n    The institution-operated surface in this repo — the Macquarie University Research Portal\n    OAI-PMH endpoint — requires NO authentication. Every verb was executed anonymously over HTTPS\n    and returned 200. There is no key, no token, no registration and no rate-limit header.\nschemes:\n- name: none\n  type: none\n  description: Anonymous HTTPS GET. Confirmed by executing all six OAI-PMH verbs with no credential.\n  evidence:\n  - url: https://research-management.mq.edu.au/ws/oai?verb=Identify\n    status: 200\n  - url: https://research-management.mq.edu.au/ws/oai?verb=ListMetadataFormats\n\
  \    status: 200\n  - url: https://research-management.mq.edu.au/ws/oai?verb=ListIdentifiers&metadataPrefix=oai_dc&set=publications:all\n    status: 200\n  sources:\n  - openapi/macquarie-research-portal-oai-pmh-openapi.yml\ntransport:\n  https: true\n  hsts: 'max-age=2592000; preload'\n  x_content_type_options: nosniff\n  observed: '2026-08-30'\nnot_covered:\n  - surface: Elsevier Pure API at https://research-management.mq.edu.au/ws/api\n    scheme: apiKey header `api-key`\n    x-operator: tenant\n    why: >-\n      The contract at /ws/api is Elsevier's — info.title \"Pure API\", contact\n      pure-support@elsevier.com, version 5.33.3-3, relative servers url /ws/api. It is a vendor\n      product spec served from a tenant host and is deliberately not described in this repo. Its\n      auth scheme is recorded here only so the absence is not mistaken for an oversight.\n  - surface: Macquarie University Research Data Repository at https://figshare.mq.edu.au\n    scheme: Figshare OAuth 2.0\
  \ (authorizationCode) on api.figshare.com\n    x-operator: tenant\n    why: >-\n      Figshare's generic OAuth, shared by every Figshare for Institutions customer. Removed from\n      this repo on 2026-08-30 along with the Figshare contract it was derived from.\n  - surface: Shibboleth IdP at https://idp.mq.edu.au/idp/shibboleth\n    scheme: SAML 2.0 (institution-operated)\n    x-operator: institution\n    why: >-\n      A federated browser SSO profile, not an HTTP API auth scheme. Recorded as an\n      IdentityFederation surface and in conformance/macquarie-domain-standards.yml instead.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/macquarie/refs/heads/main/authentication/macquarie-authentication.yml
summary_line: none · 1 scheme
tags:
- University
- Higher Education
- Education
- Australia
- Group of Eight Peer
- Research Data
- Research Repository
- Metadata Harvesting
- OAI-PMH
- Identity Federation
- Library
- Course Catalog
---
