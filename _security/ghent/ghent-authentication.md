---
api_key_in: []
api_specs:
- filename: ghent-biblio-openapi.yml
  format: yaml
  label: Ghent University Academic Bibliography API
  slug: biblio
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ghent/refs/heads/main/openapi/ghent-biblio-openapi.yml
- filename: ghent-biblio-openapi.yml
  format: yaml
  label: Ghent University Academic Bibliography OAI-PMH
  slug: biblio-oai
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ghent/refs/heads/main/openapi/ghent-biblio-openapi.yml
- filename: ghent-biblio-openapi.yml
  format: yaml
  label: Ghent University Academic Bibliography SRU
  slug: biblio-sru
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ghent/refs/heads/main/openapi/ghent-biblio-openapi.yml
- filename: ghent-hydra-resto-openapi.yml
  format: yaml
  label: Hydra Resto API
  slug: hydra-resto
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ghent/refs/heads/main/openapi/ghent-hydra-resto-openapi.yml
- filename: ghent-people-service-openapi.yaml
  format: yaml
  label: Ghent University Library People Service
  slug: people-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ghent/refs/heads/main/openapi/ghent-people-service-openapi.yaml
- filename: ghent-projects-service-openapi.yaml
  format: yaml
  label: Ghent University Library Projects Service
  slug: projects-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ghent/refs/heads/main/openapi/ghent-projects-service-openapi.yaml
- filename: ghent-oai-service-openapi.yaml
  format: yaml
  label: Ghent University Library OAI Service
  slug: oai-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ghent/refs/heads/main/openapi/ghent-oai-service-openapi.yaml
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Ghent Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ghent University declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Ghent University
provider_slug: ghent
scheme_count: 0
schemes: []
slug: ghent-authentication
source_filename: ghent-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-01'\nmethod: probed\nsource: https://biblio.ugent.be/doc/api\nx-operator: institution\nnote: >-\n  How each Ghent University surface authenticates. Verified by live probe on 2026-09-01\n  except where a contract is cited. No credential, key-request flow or OAuth endpoint was\n  invented; where a surface is genuinely open, that is recorded as open.\nsurfaces:\n  - surface: Ghent University Academic Bibliography (REST search, exports, OAI-PMH, SRU, unAPI, feeds, dumps)\n    base_url: https://biblio.ugent.be\n    scheme: none\n    public: true\n    detail: >-\n      No API key, token or registration. Anonymous GET returned 200 on the search API, both\n      OAI-PMH verbs, SRU searchRetrieve, unAPI, the sitemap index and the RSS feeds.\n      Metadata is licensed ODbL, so reuse is permitted with attribution and share-alike.\n    evidence:\n      - { url: 'https://biblio.ugent.be/publication?q=dna&format=json', status: 200 }\n      - { url: 'https://biblio.ugent.be/oai?verb=Identify',\
  \ status: 200 }\n      - { url: 'https://biblio.ugent.be/sru?version=1.1&operation=searchRetrieve&query=dna', status: 200 }\n  - surface: Hydra Resto API\n    base_url: https://hydra.ugent.be/api/2.0/resto\n    scheme: none\n    public: true\n    detail: Anonymous GET returned 200 on every documented endpoint.\n    evidence:\n      - { url: 'https://hydra.ugent.be/api/2.0/resto/meta.json', status: 200 }\n      - { url: 'https://hydra.ugent.be/api/2.0/resto/menu/en/2026/9/1.json', status: 200 }\n  - surface: People Service\n    contract: openapi/ghent-people-service-openapi.yaml\n    scheme: apiKey\n    location: header\n    parameter_name: X-Api-Key\n    public: false\n    detail: >-\n      Stated in the service's own README - PEOPLE_API_KEY is \"used in authentication header\n      X-Api-Key for server (openapi)\". The service is deployed inside the university estate;\n      no public base URL is published and no key issuance process is public.\n    evidence:\n      - { url: 'https://raw.githubusercontent.com/ugent-library/people-service/main/README.md',\
  \ status: 200 }\n  - surface: Projects Service\n    contract: openapi/ghent-projects-service-openapi.yaml\n    scheme: apiKey\n    public: false\n    detail: PROJECTS_API_KEY is a required environment variable named \"REST API Key\" in the service README.\n    evidence:\n      - { url: 'https://raw.githubusercontent.com/ugent-library/projects-service/main/README.md', status: 200 }\n  - surface: OAI Service (administrative write API behind the bibliography's OAI-PMH endpoint)\n    contract: openapi/ghent-oai-service-openapi.yaml\n    scheme: unknown\n    public: false\n    detail: >-\n      The contract declares no securitySchemes. The operations are all writes\n      (add-metadata-format, add-set, add-item, add-record, delete-record) against an internal\n      deployment, so an unauthenticated public deployment is not implied. Recorded as unknown\n      rather than none.\n  - surface: Ghent University SAML 2.0 Identity Provider\n    base_url: https://identity.ugent.be/simplesaml/saml2/idp/metadata.php\n\
  \    scheme: saml2\n    public: true\n    detail: >-\n      Metadata document is publicly readable and signed; authentication through it is\n      federated via the Belnet R&E Federation. This is the institution's own IdP, operated by\n      Directie ICT.\n    evidence:\n      - { url: 'https://identity.ugent.be/simplesaml/saml2/idp/metadata.php', status: 200 }\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ghent/refs/heads/main/authentication/ghent-authentication.yml
summary_line: 0 schemes
tags:
- University
- Higher Education
- Education
- Research
- Research Data
- Library
- Open Data
- Identity Federation
- OAI-PMH
- Belgium
- Flanders
- Europe
---
