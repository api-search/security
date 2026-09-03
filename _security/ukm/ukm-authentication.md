---
api_key_in: []
api_specs:
- filename: ukm-identity-federation-openapi.yml
  format: yaml
  label: SSO@UKM — SAML 2.0 Identity Provider
  slug: identity-federation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ukm/refs/heads/main/openapi/ukm-identity-federation-openapi.yml
- filename: ukm-ptsl-digital-oai-pmh-openapi.yml
  format: yaml
  label: UKM Learning and Research Repository (OAI-PMH)
  slug: learning-research-repository-oai
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ukm/refs/heads/main/openapi/ukm-ptsl-digital-oai-pmh-openapi.yml
- filename: ukm-ejournal-oai-pmh-openapi.yml
  format: yaml
  label: UKM e-Journal System (OAI-PMH)
  slug: ejournal-oai
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ukm/refs/heads/main/openapi/ukm-ejournal-oai-pmh-openapi.yml
- filename: ukm-web-content-rest-openapi.yml
  format: yaml
  label: UKM Web Content REST API (WordPress wp/v2)
  slug: web-content-rest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ukm/refs/heads/main/openapi/ukm-web-content-rest-openapi.yml
auth_types: []
description: How authentication works on the surfaces UKM itself operates. Derived by API Evangelist from live probes on 2026-09-01; UKM publishes no authentication documentation for any of them.
kind: authentication
layout: security
method: probed
name: Ukm Authentication
name_suffix: Authentication
oauth_flows: []
overview: Universiti Kebangsaan Malaysia declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Universiti Kebangsaan Malaysia
provider_slug: ukm
scheme_count: 0
schemes: []
slug: ukm-authentication
source_filename: ukm-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "---\nname: Universiti Kebangsaan Malaysia — authentication\ndescription: >-\n  How authentication works on the surfaces UKM itself operates. Derived by API Evangelist from live\n  probes on 2026-09-01; UKM publishes no authentication documentation for any of them.\ngenerated: '2026-09-01'\nmethod: probed\nsource: live probes of ptsldigital.ukm.my, ejournal.ukm.my, www.ukm.my and sso.ukm.my\nauthentication:\n  - surface: UKM Learning and Research Repository OAI-PMH\n    baseURL: https://ptsldigital.ukm.my/oai/request\n    x-operator: institution\n    type: none\n    detail: >-\n      Unauthenticated. All six OAI-PMH verbs answer without credentials, headers or an API key.\n      No key registration exists. Deposit and administration are behind the DSpace 6.3 login,\n      which is not part of this surface.\n  - surface: UKM e-Journal System OAI-PMH\n    baseURL: https://ejournal.ukm.my/index.php/index/oai\n    x-operator: institution\n    type: none\n    detail: >-\n      Unauthenticated.\
  \ OJS 2.4.8.1 exposes no REST API and no token issuance; /api/v1/contexts\n      returns 404.\n  - surface: UKM Web Content REST API (WordPress wp/v2)\n    baseURL: https://www.ukm.my/portal/wp-json\n    x-operator: institution\n    type: none\n    detail: >-\n      Unauthenticated for reads. The discovery document reports `authentication: []`, meaning no\n      authentication handler is registered for the REST API — cookie plus nonce is the only path\n      for writes and is available to logged-in browser sessions only. There is no application\n      password, OAuth or API key surface for third parties.\n  - surface: SSO@UKM SAML 2.0 identity provider\n    baseURL: https://sso.ukm.my/saml2/idp\n    x-operator: institution\n    type: saml2\n    detail: >-\n      This surface IS the university's authentication. Metadata retrieval is unauthenticated;\n      the SSO and SLO endpoints implement SAML 2.0 Web Browser SSO over the HTTP-Redirect binding\n      and are interactive — a non-browser\
  \ agent cannot complete the flow. Only the transient\n      NameID format is offered, so a relying party receives no stable subject identifier from the\n      NameID alone. There is no self-service relying-party registration and no dynamic client\n      registration; onboarding a service provider is an administrative process handled by\n      server@ukm.edu.my.\n    endpoints:\n      metadata: https://sso.ukm.my/saml2/idp/metadata.php\n      sso: https://sso.ukm.my/saml2/idp/SSOService.php\n      slo: https://sso.ukm.my/saml2/idp/SingleLogoutService.php\ngaps:\n  - No API key, OAuth 2.0 or OpenID Connect surface exists anywhere on UKM's own domain.\n    https://sso.ukm.my/.well-known/openid-configuration returns 404.\n  - No documented terms govern automated access to any of the unauthenticated surfaces above.\n  - Staff and student services (appsmu.ukm.my, erep.ukm.my, libquest.ukm.my) sit behind SSO@UKM and\n    are not open to third parties.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ukm/refs/heads/main/authentication/ukm-authentication.yml
summary_line: 0 schemes
tags:
- University
- Higher Education
- Education
- Research
- Malaysia
- Southeast Asia
- Identity Federation
- SAML
- Research Repository
- Institutional Repository
- OAI-PMH
- Open Access
- Scholarly Publishing
- Library
- Theses
---
