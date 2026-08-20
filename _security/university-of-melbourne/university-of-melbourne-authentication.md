---
api_key_in: []
api_specs:
- filename: university-of-melbourne-sudo-geonode-openapi.yml
  format: yaml
  label: Spatial Urban Data Observatory (SUDO) API
  slug: sudo-spatial-urban-data-observatory
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-melbourne/refs/heads/main/openapi/university-of-melbourne-sudo-geonode-openapi.yml
- filename: university-of-melbourne-minerva-access-dspace-openapi.yml
  format: yaml
  label: Minerva Access Repository REST API (DSpace 7.6)
  slug: minerva-access-rest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-melbourne/refs/heads/main/openapi/university-of-melbourne-minerva-access-dspace-openapi.yml
- filename: university-of-melbourne-minerva-access-oai-pmh-openapi.yml
  format: yaml
  label: Minerva Access OAI-PMH 2.0 Endpoint
  slug: minerva-access-oai-pmh
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-melbourne/refs/heads/main/openapi/university-of-melbourne-minerva-access-oai-pmh-openapi.yml
auth_types: []
description: 'Authentication posture per surface, split by operator. The University of Melbourne runs two distinct identity systems and neither is an API product: a self-hosted Shibboleth SAML 2.0 IdP for federated research and library access (institution-operated), and an Okta tenancy on a University vanity hostname for web SSO (tenant). Its two publicly callable read APIs require no authentication at all.'
kind: authentication
layout: security
method: probed
name: University Of Melbourne Authentication
name_suffix: Authentication
oauth_flows: []
overview: University of Melbourne declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: University of Melbourne
provider_slug: university-of-melbourne
scheme_count: 0
schemes: []
slug: university-of-melbourne-authentication
source_filename: university-of-melbourne-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-19'\nmethod: probed\nsource: >-\n  Live probes on 2026-08-19 of each surface listed below; request/response\n  statuses recorded per entry.\ndescription: >-\n  Authentication posture per surface, split by operator. The University of\n  Melbourne runs two distinct identity systems and neither is an API product:\n  a self-hosted Shibboleth SAML 2.0 IdP for federated research and library\n  access (institution-operated), and an Okta tenancy on a University vanity\n  hostname for web SSO (tenant). Its two publicly callable read APIs require\n  no authentication at all.\nsurfaces:\n  - name: Spatial Urban Data Observatory (SUDO) API v2\n    url: https://sudo.eresearch.unimelb.edu.au/api/v2\n    x-operator: institution\n    type: none\n    verified: '2026-08-19'\n    detail: >-\n      Anonymous GET returns 200. Response headers show\n      `Allow: GET, HEAD, OPTIONS`, `access-control-allow-origin: *`,\n      `Access-Control-Allow-Credentials: false`, and\n   \
  \   `Access-Control-Allow-Headers: Content-Type, Accept, Authorization,\n      Origin, User-Agent` — so an Authorization header is accepted for\n      write/private scopes but is not required to read. A Django `sessionid`\n      cookie is set on every anonymous request. No API-key issuance, no\n      registration, no published rate limit.\n  - name: Minerva Access DSpace REST API\n    url: https://minerva-access.unimelb.edu.au/server/api\n    x-operator: institution\n    type: none\n    verified: '2026-08-19'\n    detail: >-\n      Anonymous GET returns 200 for public content. DSpace 7.6 advertises an\n      `authn` and an `oidc` link relation from its root document for\n      authenticated operations, but reading communities, collections and items\n      requires no credential.\n  - name: Minerva Access OAI-PMH\n    url: https://minerva-access.unimelb.edu.au/server/oai/request\n    x-operator: institution\n    type: none\n    verified: '2026-08-19'\n    detail: Open harvesting interface,\
  \ no credential of any kind.\n  - name: Shibboleth Identity Provider\n    url: https://idp.unimelb.edu.au/idp/shibboleth\n    x-operator: institution\n    type: saml2\n    verified: '2026-08-19'\n    detail: >-\n      Self-hosted Shibboleth IdP. Metadata is public (200 application/xml) and\n      registered in the Australian Access Federation aggregate; the\n      authentication itself is federated SAML 2.0 for members of scope\n      `unimelb.edu.au`. SSO endpoints:\n      https://idp.unimelb.edu.au/idp/profile/SAML2/Redirect/SSO,\n      /SAML2/POST/SSO, /SAML2/POST-SimpleSign/SSO.\n      This is the institution's own identity engineering — not a purchased\n      contract — and it is the single most consequential machine-readable\n      surface it operates.\n  - name: University SSO (Okta)\n    url: https://sso.unimelb.edu.au\n    x-operator: tenant\n    type: oauth2/oidc\n    verified: '2026-08-19'\n    detail: >-\n      OpenID Connect discovery and RFC 8414 metadata both return 200.\n\
  \      Issuer https://sso.unimelb.edu.au. Endpoints /oauth2/v1/authorize,\n      /oauth2/v1/token, /oauth2/v1/userinfo, /oauth2/v1/clients. Okta operates\n      the platform — grant_types_supported carries\n      urn:okta:params:oauth:grant-type:otp / :oob and Auth0 MFA grant URNs —\n      under a University hostname. Client registration is not open to the\n      public; there is no developer sign-up.\n  - name: Spartan HPC dashboard\n    url: https://dashboard.hpc.unimelb.edu.au\n    x-operator: institution\n    type: saml2\n    verified: '2026-08-19'\n    detail: >-\n      Registered as a Shibboleth Service Provider in the AAF aggregate\n      (entityID https://dashboard.hpc.unimelb.edu.au/shibboleth). The\n      unauthenticated web root now redirects to a Confluence knowledge base on\n      rcs-knowledge-hub.atlassian.net, so the dashboard itself is gated behind\n      federated login and no API surface is publicly observable.\n  - name: Melbourne Data research repository\n    url:\
  \ https://melbourne.figshare.com\n    x-operator: tenant\n    type: unknown\n    verified: '2026-08-19'\n    detail: >-\n      Returned HTTP 202 with an AWS WAF JavaScript challenge body rather than\n      content. Bot-challenged, therefore live; authentication posture not\n      determinable. The Figshare API is Figshare's contract and is deliberately\n      not saved in this repository.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-melbourne/refs/heads/main/authentication/university-of-melbourne-authentication.yml
summary_line: 0 schemes
tags:
- University
- Higher Education
- Education
- Australia
- Group of Eight
- Research
- Research Data
- Research Repository
- Open Data
- Geospatial
- Identity Federation
- Library
---
