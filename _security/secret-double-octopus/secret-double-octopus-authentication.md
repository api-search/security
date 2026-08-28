---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Secret Double Octopus Authentication
name_suffix: Authentication
oauth_flows: []
overview: Secret Double Octopus declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Secret Double Octopus
provider_slug: secret-double-octopus
scheme_count: 0
schemes: []
slug: secret-double-octopus-authentication
source_filename: secret-double-octopus-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: >-\n  https://support.doubleoctopus.com/support/solutions/articles/33000275542-how-to-configure-the-help-desk-role,\n  https://support.doubleoctopus.com/support/solutions/articles/33000294232-frequently-ask-questions,\n  https://docs.pingidentity.com/auth-node-ref/latest/cloud/secret-double-octopus.html\ndocs: https://support.doubleoctopus.com/support/solutions/articles/33000275542-how-to-configure-the-help-desk-role\napi: Octopus Management Console REST API\nnote: >-\n  DERIVATION IMPOSSIBLE: SDO publishes no OpenAPI, so no securityScheme could be read. Everything\n  below is read from SDO's public support articles and from identity-vendor integration docs that\n  describe configuring against a real Octopus server. It is a description of the documented auth\n  model, not a transcription of a spec.\nsecurity_schemes:\n- id: octopus_api_token\n  type: apiKey\n  in: header\n  documented_as: API Token\n  description: >-\n    A\
  \ REST API service is created in the Octopus Management Console; the resulting API Token is read\n    from the Sign On tab of that service (\"click View, then Copy\"). Integrations are configured with\n    three values together — the API token, the service URL, and the service certificate.\n  issued_by: Octopus Management Console (admin creates a REST API service)\n  rotation: not-published\n  header_name: not-published\n  evidence:\n  - https://docs.pingidentity.com/auth-node-ref/latest/cloud/secret-double-octopus.html\n  - https://github.com/ForgeRock/Secret-Double-Octopus-Auth-Tree-Node\n- id: service_certificate\n  type: mutualTLS\n  documented_as: service certificate\n  description: >-\n    Integrations are given a service certificate alongside the API token and service URL, so the\n    channel to the Octopus server is certificate-pinned/mTLS in addition to the token.\n  evidence:\n  - https://docs.pingidentity.com/auth-node-ref/latest/cloud/secret-double-octopus.html\noauth2: false\n\
  openid_connect:\n  supported: true\n  role: >-\n    SDO acts as an identity/authentication provider TO applications over OIDC, SAML, WS-Federation,\n    WS-Trust and RADIUS. That is the product's application-integration surface, not the auth model\n    of the Management Console REST API, which uses the API token above.\n  discovery_document: not-published\n  note: >-\n    No /.well-known/openid-configuration is served on any SDO-controlled host — the OIDC issuer is\n    each customer's own deployed Octopus server, not a vendor host.\nauthorization:\n  model: role-based, resource+method ACL\n  description: >-\n    Console roles are scoped with JSON rules of the form\n    {\"resource\": \"<REST API URL>\", \"methods\": [\"<Method1>\", \"<Method2>\"], \"action\": \"<allow/deny>\"},\n    where the resource string is only the portion of the URL following <URL>:<port>/api/. The\n    permissible resource/method pairs are enumerated on the deployment's own REST API reference at\n    <URL>:<port>/docs/.\n\
  \  evidence: https://support.doubleoctopus.com/support/solutions/articles/33000275542-how-to-configure-the-help-desk-role\n  scopes_artifact: not-applicable\nend_user_authenticators:\n- mobile push (Octopus Authenticator, iOS and Android)\n- biometrics / facial\n- FIDO2 security keys\n- X.509 smart cards\n- Windows Hello\n- OTP tokens\n- Bluetooth Low Energy offline authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/secret-double-octopus/refs/heads/main/authentication/secret-double-octopus-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Authentication
- Identity and Access Management
- Passwordless
- Multi-Factor Authentication
- Security
- FIDO2
- Zero Trust
- Enterprise
- Workforce Identity
---
