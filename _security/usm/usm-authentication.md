---
api_key_in: []
api_specs:
- filename: usm-repository-oai-pmh-openapi.yml
  format: yaml
  label: USM Repository OAI-PMH
  slug: eprints-oai
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usm/refs/heads/main/openapi/usm-repository-oai-pmh-openapi.yml
- filename: usm-repository-eprints-rest-openapi.yml
  format: yaml
  label: USM Repository EPrints REST and Export
  slug: eprints-rest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usm/refs/heads/main/openapi/usm-repository-eprints-rest-openapi.yml
auth_types: []
description: How each Universiti Sains Malaysia surface authenticates, established by probing the live hosts on 2026-09-01. USM publishes no developer authentication documentation of any kind; every statement below comes from an observed response.
kind: authentication
layout: security
method: probed
name: Usm Authentication
name_suffix: Authentication
oauth_flows: []
overview: Universiti Sains Malaysia declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Universiti Sains Malaysia
provider_slug: usm
scheme_count: 0
schemes: []
slug: usm-authentication
source_filename: usm-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "---\nname: Universiti Sains Malaysia authentication posture\ndescription: >-\n  How each Universiti Sains Malaysia surface authenticates, established by probing the\n  live hosts on 2026-09-01. USM publishes no developer authentication documentation of\n  any kind; every statement below comes from an observed response.\ngenerated: '2026-09-01'\nmethod: probed\nsource: https://eprints.usm.my/ , https://shibsso.usm.my/ , https://api.usm.my/ , https://elearning.usm.my/\nsurfaces:\n  - surface: Repository@USM OAI-PMH\n    url: https://eprints.usm.my/cgi/oai2\n    x-operator: institution\n    scheme: none\n    detail: >-\n      Anonymous read. No key, token, referrer or User-Agent condition observed; the\n      endpoint answered an unauthenticated Identify, ListMetadataFormats, ListSets and\n      ListIdentifiers on 2026-09-01.\n    evidence:\n      - url: https://eprints.usm.my/cgi/oai2?verb=Identify\n        status: 200\n  - surface: Repository@USM EPrints REST + export plugins\n\
  \    url: https://eprints.usm.my/rest/\n    x-operator: institution\n    scheme: none\n    detail: >-\n      Anonymous read across /rest/eprint/, /rest/subject/ and /cgi/export/. Write\n      operations exist in EPrints but are not exposed to unauthenticated clients and\n      were not probed. No signup, key issuance or rate-limit header was observed.\n    evidence:\n      - url: https://eprints.usm.my/rest/\n        status: 200\n      - url: https://eprints.usm.my/rest/eprint/16.xml\n        status: 200\n  - surface: USM Shibboleth Identity Provider\n    url: https://shibsso.usm.my/idp/shibboleth\n    x-operator: federation\n    scheme: saml2\n    detail: >-\n      USM's own SAML 2.0 / Shibboleth IdP, registered in the SIFULAN Malaysian Access\n      Federation on 2021-10-30 and exported to eduGAIN. Scope usm.my. Carries the\n      REFEDS Research and Scholarship entity category. SSO bindings published:\n      HTTP-POST, HTTP-Redirect, POST-SimpleSign and the Shibboleth 1.0 AuthnRequest\n\
  \      profile; SLO over POST, Redirect and SOAP; an AttributeAuthority over SAML1 and\n      SAML2 SOAP. This is the institution's strongest machine-readable identity surface\n      and it is in live use — eduvpn.usm.my redirects an unauthenticated request\n      straight into https://shibsso.usm.my/idp/profile/SAML2/Redirect/SSO.\n    evidence:\n      - url: https://metadata.sifulan.my/metadata.xml\n        status: 200\n      - url: https://shibsso.usm.my/idp/shibboleth\n        status: 200\n      - url: https://eduvpn.usm.my/\n        status: 200\n  - surface: API@USM portal\n    url: https://api.usm.my/\n    x-operator: institution\n    scheme: unknown\n    detail: >-\n      The page renders login and register modals, but the whole site is an unmodified\n      TemplateMo \"Chain App Dev\" HTML template — body copy is lorem ipsum, the contact\n      address is the template's own info@company.co, and every navigation link is an\n      in-page anchor. No authentication endpoint, no catalog\
  \ and no documentation path\n      exists behind it (/docs, /openapi.json, /swagger-ui and /robots.txt all 404).\n      Treat the login as scaffolding, not as a gate in front of an API programme.\n    evidence:\n      - url: https://api.usm.my/\n        status: 200\n      - url: https://api.usm.my/openapi.json\n        status: 404\n      - url: https://api.usm.my/docs\n        status: 404\n  - surface: USM Moodle (e-Learning@USM)\n    url: https://elearning.usm.my/sidang2526/\n    x-operator: institution\n    scheme: token\n    detail: >-\n      Self-hosted Moodle with the REST web-service server enabled. An unauthenticated\n      call returns Moodle's own invalidtoken exception, which proves the service is\n      live and token-gated. The contract is Moodle's, not USM's — the deployment and\n      the host are USM's.\n    evidence:\n      - url: https://elearning.usm.my/sidang2526/webservice/rest/server.php?wstoken=x&wsfunction=core_webservice_get_site_info&moodlewsrestformat=json\n \
  \       status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/usm/refs/heads/main/authentication/usm-authentication.yml
summary_line: 0 schemes
tags:
- University
- Higher Education
- Education
- Public Research University
- Malaysia
- Southeast Asia
- Research
- Open Access
- Institutional Repository
- OAI-PMH
- EPrints
- Identity Federation
- Shibboleth
- SAML
- Crossref
---
