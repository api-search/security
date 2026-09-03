---
api_key_in: []
auth_types: []
description: 'Tianjin University publishes no public API, so there is no API key, token, OAuth client or self-service registration to describe. What it does operate is institutional authentication: a Shibboleth SAML 2.0 identity provider used for federated access to licensed resources through CARSI, and a campus-network access control that fronts most internal systems.'
kind: authentication
layout: security
method: probed
name: Tianjin Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tianjin University declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Tianjin University
provider_slug: tianjin
scheme_count: 0
schemes: []
slug: tianjin-authentication
source_filename: tianjin-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "specification: API Evangelist Authentication Profile\nspecificationVersion: '0.1'\nprovider: Tianjin University\nproviderId: tianjin\ngenerated: '2026-09-01'\nmethod: probed\nsource: >-\n  https://idp.tju.edu.cn/idp/shibboleth (HTTP 200, archived under identity-federation/);\n  https://idp.tju.edu.cn/idp/profile/SAML2/Redirect/SSO (HTTP 400, branded Shibboleth error page);\n  https://idp.tju.edu.cn/idp/status (HTTP 403); negative probes of\n  https://idp.tju.edu.cn/.well-known/openid-configuration and\n  https://idp.tju.edu.cn/idp/profile/oidc/keyset (both HTTP 404); and the CARSI entity record in\n  the eduGAIN technical entity list.\ndescription: >-\n  Tianjin University publishes no public API, so there is no API key, token, OAuth client or\n  self-service registration to describe. What it does operate is institutional authentication:\n  a Shibboleth SAML 2.0 identity provider used for federated access to licensed resources through\n  CARSI, and a campus-network access control\
  \ that fronts most internal systems.\n\napi_authentication:\n  public_api: false\n  schemes: []\n  registration: none\n  detail: >-\n    No developer portal, no API key issuance, no OAuth or OIDC authorization server offered to\n    third parties, and no documented API authentication of any kind on any tju.edu.cn host.\n\ninstitutional_authentication:\n- name: Tianjin University Shibboleth IdP (CARSI)\n  protocol: SAML 2.0 (Shibboleth)\n  entity_id: https://idp.tju.edu.cn/idp/shibboleth\n  metadata: identity-federation/tianjin-idp-saml-metadata.xml\n  federation: CARSI / eduGAIN\n  x-operator: institution\n  audience: >-\n    University members authenticating to CARSI-federated service providers — chiefly licensed\n    library and publisher resources. Not a third-party developer surface: relying parties join by\n    federation registration, not by signing up.\n  bindings:\n  - urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect\n  - urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST\n  - urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST-SimpleSign\n\
  \  - urn:oasis:names:tc:SAML:2.0:bindings:SOAP\n  - urn:mace:shibboleth:1.0:profiles:AuthnRequest\n  oidc: absent\n  oidc_evidence:\n  - url: https://idp.tju.edu.cn/.well-known/openid-configuration\n    status: 404\n  - url: https://idp.tju.edu.cn/idp/profile/oidc/keyset\n    status: 404\n\nnetwork_access_control:\n  name: TJU campus-network gate\n  host: network-notice.tju.edu.cn\n  behaviour: >-\n    Off-campus requests to several university systems are transparently redirected to\n    http://network-notice.tju.edu.cn/, which serves a page titled \"403\" with HTTP status 200 — a\n    soft-403. It is an access control, not an outage, and the hosts behind it are graded live.\n  x-operator: institution\n  observed_on:\n  - host: opac.lib.tju.edu.cn\n    a_record: 202.113.2.196\n  - host: ir.lib.tju.edu.cn\n    a_record: 202.113.2.196\n  - host: portal.tju.edu.cn\n    a_record: 202.113.2.198\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tianjin/refs/heads/main/authentication/tianjin-authentication.yml
summary_line: 0 schemes
tags:
- Education
- Higher Education
- University
- Research
- China
- Tianjin
- Double First Class
- Project 985
- Identity Federation
- Shibboleth
- SAML
- Single Sign-On
- Library
- Research Repository
- Persistent Identifiers
---
