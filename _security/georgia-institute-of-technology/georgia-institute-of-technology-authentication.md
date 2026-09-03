---
api_key_in: []
api_specs:
- filename: georgia-institute-of-technology-gtplaces-openapi.yml
  format: yaml
  label: GT Places API
  slug: gt-places
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/georgia-institute-of-technology/refs/heads/main/openapi/georgia-institute-of-technology-gtplaces-openapi.yml
- filename: georgia-institute-of-technology-api-api-openapi.yml
  format: yaml
  label: Georgia Tech SUMS REST API
  slug: sums
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/georgia-institute-of-technology/refs/heads/main/openapi/georgia-institute-of-technology-api-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Georgia Institute Of Technology Authentication
name_suffix: Authentication
oauth_flows: []
overview: Georgia Institute of Technology declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Georgia Institute of Technology
provider_slug: georgia-institute-of-technology
scheme_count: 0
schemes: []
slug: georgia-institute-of-technology-authentication
source_filename: georgia-institute-of-technology-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-01'\nmethod: probed\nsource: >-\n  Live unauthenticated probes of Georgia Institute of Technology hosts on 2026-09-01. Every row below\n  records what an anonymous client actually received; nothing is inferred from documentation prose.\nnote: >-\n  Georgia Tech operates no central developer portal and issues no self-service API keys on any public\n  surface. Authentication across the institution's programmable surfaces is one of three things:\n  nothing at all (the library repository), CAS/Shibboleth single sign-on for humans, or an\n  institutional credential negotiated offline (BuzzAPI, SUMS). Where a documentation page and the\n  deployed endpoint disagree, the deployed endpoint is recorded.\nsurfaces:\n- name: GT Digital Repository OAI-PMH\n  base_url: https://repository.gatech.edu/server/oai/request\n  x-operator: institution\n  scheme: none\n  anonymous_access: true\n  evidence: verb=Identify, verb=ListMetadataFormats and verb=ListSets all return 200\
  \ text/xml with no credentials.\n- name: GT Digital Repository REST API (DSpace 7.6)\n  base_url: https://repository.gatech.edu/server/api\n  x-operator: institution\n  scheme: none\n  anonymous_access: true\n  evidence: >-\n    Root returns 200 application/hal+json (dspaceVersion \"DSpace 7.6\"); /core/communities returns 200\n    application/hal+json, 7,091 bytes. Write and administrative operations sit behind\n    /server/api/authn, which was not exercised. No OpenAPI is published — /server/api/openapi.json\n    returns 404.\n- name: GT Places API\n  base_url: https://m.gatech.edu/api\n  x-operator: institution\n  scheme: microsoft-entra-id\n  anonymous_access: false\n  evidence: >-\n    RNOC's documentation page states \"This API is open to all\" and \"The Api is currently live\", but\n    https://m.gatech.edu/api/gtplaces/buildings/ and /gtplaces/categories/ both return 200\n    text/html — a ~23 KB Microsoft Entra ID sign-in redirect page, not JSON. Documented as open,\n    deployed\
  \ behind institutional SSO. The contract itself remains publicly readable at\n    https://rnoc.gatech.edu/sites/default/files/gtplaces_6.yaml (200 text/plain).\n- name: Georgia Tech SUMS REST API\n  base_url: https://sums.gatech.edu/SUMSAPI/rest/API\n  x-operator: institution\n  scheme: api-key\n  anonymous_access: false\n  evidence: >-\n    The Swagger 2.0 document at https://sums.gatech.edu/SUMSAPI/rest/API/swagger.json is publicly\n    readable (200), and most operations declare a required `APIKey` query parameter. There is no\n    published registration or self-service issuance path for that key; it is obtained from the\n    operating unit.\n- name: BuzzAPI (api.gatech.edu)\n  base_url: https://api.gatech.edu/apiv3\n  x-operator: institution\n  scheme: institutional-credential\n  anonymous_access: false\n  evidence: >-\n    https://api.gatech.edu/, https://api.gatech.edu/apiv3 and https://test.api.gatech.edu/ all return\n    404 application/json to an unauthenticated client — a gateway\
  \ responding, not a dead host. The\n    developer handbook that documented BuzzAPI at webmasters.gatech.edu was removed in that site's\n    2026 rebuild (both former URLs now 404, and the site's own search returns \"Access denied\" to\n    anonymous users), so no public documentation for BuzzAPI could be found on 2026-09-01.\n- name: Shibboleth Identity Provider\n  base_url: https://idp.gatech.edu/idp/shibboleth\n  x-operator: institution\n  scheme: saml2\n  anonymous_access: true\n  evidence: >-\n    Metadata is public and unauthenticated — 200 text/xml direct from the IdP, and 200\n    application/samlmetadata+xml (signed) from InCommon MDQ. The SSO endpoint itself returns 400 to a\n    parameterless GET. This is the institution's own IdP, scoped gatech.edu.\n- name: CAS single sign-on\n  base_url: https://sso.gatech.edu/cas/login\n  x-operator: institution\n  scheme: cas\n  anonymous_access: false\n  evidence: https://sso.gatech.edu/ redirects (200) to https://sso.gatech.edu/cas/login,\
  \ a CAS login form.\nnegative_probes:\n- url: https://www.gatech.edu/.well-known/security.txt\n  status: 404\n- url: https://gatech.edu/.well-known/security.txt\n  status: 404\n- url: https://www.gatech.edu/llms.txt\n  status: 404\n- url: https://repository.gatech.edu/server/api/openapi.json\n  status: 404\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/georgia-institute-of-technology/refs/heads/main/authentication/georgia-institute-of-technology-authentication.yml
summary_line: 0 schemes
tags:
- University
- Higher Education
- Education
- United States
- Institute of Technology
- Public Research University
- Research Repository
- Identity Federation
- Course Catalog
- Library
- Open Data
- Research
---
