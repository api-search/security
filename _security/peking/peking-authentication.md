---
api_key_in: []
api_specs:
- filename: peking-institutional-repository-rest-openapi.yml
  format: yaml
  label: PKU Institutional Repository REST API
  slug: ir-rest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peking/refs/heads/main/openapi/peking-institutional-repository-rest-openapi.yml
- filename: peking-institutional-repository-oai-pmh-openapi.yml
  format: yaml
  label: PKU Institutional Repository OAI-PMH API
  slug: ir-oai-pmh
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peking/refs/heads/main/openapi/peking-institutional-repository-oai-pmh-openapi.yml
auth_types:
- saml2
- shibboleth
- cas
- oauth2
- none
description: ''
kind: authentication
layout: security
method: probed
name: Peking Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Peking University secures its APIs with saml2, shibboleth, cas, oauth2, and none across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Peking University
provider_slug: peking
scheme_count: 4
schemes:
- description: SAML 2.0 identity provider for Peking University, published as live Shibboleth metadata (14KB of XML, HTTP 200 on 2026-08-19). Declares SAML 2.0 POST, POST-SimpleSign and Redirect SSO/SLO profiles, the legacy Shibboleth SSO profile, and SOAP ArtifactResolution / AttributeQuery / SLO endpoints on port 8443. Registered in eduGAIN with registration authority https://www.carsi.edu.cn and in production since 2019-06-18.
  endpoints:
  - https://idp.pku.edu.cn/idp/profile/SAML2/POST/SSO
  - https://idp.pku.edu.cn/idp/profile/SAML2/Redirect/SSO
  - https://idp.pku.edu.cn/idp/profile/SAML2/POST-SimpleSign/SSO
  - https://idp.pku.edu.cn/idp/profile/Shibboleth/SSO
  - https://idp.pku.edu.cn:8443/idp/profile/SAML2/SOAP/AttributeQuery
  - https://idp.pku.edu.cn:8443/idp/profile/SAML2/SOAP/ArtifactResolution
  entity_id: https://idp.pku.edu.cn/idp/shibboleth
  metadata_url: https://idp.pku.edu.cn/idp/shibboleth
  name: PKU Shibboleth Identity Provider
  scope: pku.edu.cn
  sources:
  - https://idp.pku.edu.cn/idp/shibboleth
  - https://technical.edugain.org/api.php?action=list_entities
  type: saml2
- description: Peking University Computer Center operates CARSI, the CERNET Authentication and Resource Sharing Infrastructure — the national identity federation for Chinese higher education. eduGAIN's federation registry lists CARSI with the contact address carsi@pku.edu.cn, registration authority https://www.carsi.edu.cn, eduGAIN membership from 2019-05-24 and production from 2019-06-18. 1,042 SAML entities in eduGAIN carry CARSI as their registration authority, including PKU's own IdP and SP. The carsi.edu.cn site footer reads 版权所有©北京大学计算中心 (Copyright, Peking University Computer Center).
  name: CARSI federation
  sources:
  - https://www.carsi.edu.cn/
  - https://technical.edugain.org/api.php?action=list_feds
  type: saml2-federation
- description: IAAA is the campus-wide unified authentication service (CAS/SSO) at iaaa.pku.edu.cn. It fronts staff and student services and exposes an OAuth authorization entry point at /iaaa/oauth.jsp (HTTP 200 on 2026-08-19), but client registration, scope documentation and token endpoints are behind an institutional approval process. It is not a public developer API.
  name: PKU IAAA unified authentication
  sources:
  - https://iaaa.pku.edu.cn/
  - https://iaaa.pku.edu.cn/iaaa/oauth.jsp
  type: cas
- description: The Institutional Repository REST and OAI-PMH surfaces are open. No API key, token or registration was required for any read path probed on 2026-08-19.
  name: Anonymous read
  sources:
  - https://ir.pku.edu.cn/rest/status
  type: none
slug: peking-authentication
source_filename: peking-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-19'\nmethod: probed\nsource: https://idp.pku.edu.cn/idp/shibboleth\ndocs: https://iaaa.pku.edu.cn/iaaa/\nx-operator: institution\nnote: >-\n  Peking University runs its own campus identity infrastructure and its own federated\n  identity provider, and it also operates CARSI — the CERNET Authentication and Resource\n  Sharing Infrastructure — which is China's national research-and-education identity\n  federation and a full eduGAIN member. The federation is the strongest authentication\n  fact in this profile: it is machine-readable, institution-operated, and independently\n  corroborated by eduGAIN's own registry.\n\n  The public repository APIs (ir.pku.edu.cn/rest, ir.pku.edu.cn/oai) require no\n  authentication for read access — /rest/status returns authenticated=false and okay=true\n  to an anonymous caller and every read path probed on 2026-08-19 answered without\n  credentials.\nsummary:\n  types: [saml2, shibboleth, cas, oauth2, none]\n  api_key_in:\
  \ []\n  oauth2_flows: [authorizationCode]\nschemes:\n  - name: PKU Shibboleth Identity Provider\n    type: saml2\n    entity_id: https://idp.pku.edu.cn/idp/shibboleth\n    metadata_url: https://idp.pku.edu.cn/idp/shibboleth\n    scope: pku.edu.cn\n    description: >-\n      SAML 2.0 identity provider for Peking University, published as live Shibboleth\n      metadata (14KB of XML, HTTP 200 on 2026-08-19). Declares SAML 2.0 POST, POST-SimpleSign\n      and Redirect SSO/SLO profiles, the legacy Shibboleth SSO profile, and SOAP\n      ArtifactResolution / AttributeQuery / SLO endpoints on port 8443. Registered in\n      eduGAIN with registration authority https://www.carsi.edu.cn and in production\n      since 2019-06-18.\n    endpoints:\n      - https://idp.pku.edu.cn/idp/profile/SAML2/POST/SSO\n      - https://idp.pku.edu.cn/idp/profile/SAML2/Redirect/SSO\n      - https://idp.pku.edu.cn/idp/profile/SAML2/POST-SimpleSign/SSO\n      - https://idp.pku.edu.cn/idp/profile/Shibboleth/SSO\n  \
  \    - https://idp.pku.edu.cn:8443/idp/profile/SAML2/SOAP/AttributeQuery\n      - https://idp.pku.edu.cn:8443/idp/profile/SAML2/SOAP/ArtifactResolution\n    sources:\n      - https://idp.pku.edu.cn/idp/shibboleth\n      - https://technical.edugain.org/api.php?action=list_entities\n  - name: CARSI federation\n    type: saml2-federation\n    description: >-\n      Peking University Computer Center operates CARSI, the CERNET Authentication and\n      Resource Sharing Infrastructure — the national identity federation for Chinese\n      higher education. eduGAIN's federation registry lists CARSI with the contact\n      address carsi@pku.edu.cn, registration authority https://www.carsi.edu.cn,\n      eduGAIN membership from 2019-05-24 and production from 2019-06-18. 1,042 SAML\n      entities in eduGAIN carry CARSI as their registration authority, including PKU's\n      own IdP and SP. The carsi.edu.cn site footer reads 版权所有©北京大学计算中心\n      (Copyright, Peking University Computer Center).\n \
  \   sources:\n      - https://www.carsi.edu.cn/\n      - https://technical.edugain.org/api.php?action=list_feds\n  - name: PKU IAAA unified authentication\n    type: cas\n    description: >-\n      IAAA is the campus-wide unified authentication service (CAS/SSO) at\n      iaaa.pku.edu.cn. It fronts staff and student services and exposes an OAuth\n      authorization entry point at /iaaa/oauth.jsp (HTTP 200 on 2026-08-19), but client\n      registration, scope documentation and token endpoints are behind an institutional\n      approval process. It is not a public developer API.\n    sources:\n      - https://iaaa.pku.edu.cn/\n      - https://iaaa.pku.edu.cn/iaaa/oauth.jsp\n  - name: Anonymous read\n    type: none\n    description: >-\n      The Institutional Repository REST and OAI-PMH surfaces are open. No API key,\n      token or registration was required for any read path probed on 2026-08-19.\n    sources:\n      - https://ir.pku.edu.cn/rest/status\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/peking/refs/heads/main/authentication/peking-authentication.yml
summary_line: saml2/shibboleth/cas/oauth2/none · 4 schemes
tags:
- University
- Higher Education
- Education
- China
- Public Research University
- C9 League
- Research Repository
- Identity Federation
- Research Data
- Open Data
- Research Computing
- OAI-PMH
---
