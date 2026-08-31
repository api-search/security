---
api_key_in: []
auth_types: []
description: United Arab Emirates University operates its own enterprise identity service at eisprod.uaeu.ac.ae. It is the single sign-on point for university applications — Banner Self-Service at ssb.uaeu.ac.ae redirects into it — and it publishes three unauthenticated, standards-mandated discovery documents. This is the only machine-readable surface UAEU itself operates; it is not an API product and there is no developer program behind it.
kind: authentication
layout: security
method: probed
name: United Arab Emirates University Authentication
name_suffix: Authentication
oauth_flows: []
overview: United Arab Emirates University declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: United Arab Emirates University
provider_slug: united-arab-emirates-university
scheme_count: 0
schemes: []
slug: united-arab-emirates-university-authentication
source_filename: united-arab-emirates-university-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "---\naid: united-arab-emirates-university\nname: United Arab Emirates University — Authentication\ngenerated: '2026-08-30'\nmethod: probed\nsource: https://eisprod.uaeu.ac.ae/oauth2/oidcdiscovery/.well-known/openid-configuration\nx-operator: institution\noperator_evidence: >-\n  eisprod.uaeu.ac.ae resolves under the institution's own registrable domain\n  uaeu.ac.ae and presents a GoDaddy-issued wildcard certificate for\n  CN=*.uaeu.ac.ae (SAN *.uaeu.ac.ae, uaeu.ac.ae). The SAML 2.0 EntityDescriptor\n  carries entityID \"eisprod.uaeu.ac.ae\". No vendor host, contact domain or\n  service mark appears in any of the three discovery documents. The underlying\n  product is WSO2 Identity Server, but the deployment, the domain, the\n  certificate and the identity data are the university's.\ndescription: >-\n  United Arab Emirates University operates its own enterprise identity service\n  at eisprod.uaeu.ac.ae. It is the single sign-on point for university\n  applications — Banner\
  \ Self-Service at ssb.uaeu.ac.ae redirects into it — and\n  it publishes three unauthenticated, standards-mandated discovery documents.\n  This is the only machine-readable surface UAEU itself operates; it is not an\n  API product and there is no developer program behind it.\nmechanisms:\n  - type: openid-connect\n    status: live\n    discovery: https://eisprod.uaeu.ac.ae/oauth2/oidcdiscovery/.well-known/openid-configuration\n    http_status: 200\n    content_type: application/json\n    issuer: https://eisprod.uaeu.ac.ae:9443/oauth2endpoints/token\n    endpoints:\n      authorization: https://eisprod.uaeu.ac.ae:443/oauth2/authorize\n      token: https://eisprod.uaeu.ac.ae:443/oauth2/token\n      userinfo: https://eisprod.uaeu.ac.ae:443/oauth2/userinfo\n      introspection: https://eisprod.uaeu.ac.ae:443/oauth2/introspect\n      revocation: https://eisprod.uaeu.ac.ae:443/oauth2/revoke\n      end_session: https://eisprod.uaeu.ac.ae:443/oidc/logout\n      jwks: https://eisprod.uaeu.ac.ae:443/oauth2/jwks\n\
  \      registration: https://eisprod.uaeu.ac.ae:443/api/identity/oauth2/dcr/v1.1/register\n    grant_types:\n      - authorization_code\n      - client_credentials\n      - password\n      - refresh_token\n      - urn:ietf:params:oauth:grant-type:device_code\n      - urn:ietf:params:oauth:grant-type:jwt-bearer\n      - urn:ietf:params:oauth:grant-type:saml2-bearer\n      - urn:ietf:params:oauth:grant-type:uma-ticket\n    pkce: [ S256, plain ]\n    id_token_signing: [ RS256 ]\n    subject_types: [ pairwise ]\n    notes: >-\n      Dynamic client registration (RFC 7591) is advertised at the DCR endpoint\n      but was not exercised. The discovery document is readable without\n      credentials; every operational endpoint behind it requires a registered\n      client.\n  - type: saml2\n    status: live\n    metadata: https://eisprod.uaeu.ac.ae/identity/metadata/saml2\n    http_status: 200\n    content_type: application/xml\n    entity_id: eisprod.uaeu.ac.ae\n    role: IDPSSODescriptor\n  \
  \  protocol_support: urn:oasis:names:tc:SAML:2.0:protocol\n    want_authn_requests_signed: false\n    notes: >-\n      Institution-operated SAML 2.0 identity provider metadata. This is an\n      IdP metadata document, NOT an eduGAIN or InCommon federation entry — no\n      evidence of UAEU participation in a multilateral R&E federation was found,\n      and none is claimed here.\n  - type: scim2\n    status: partial\n    service_provider_config: https://eisprod.uaeu.ac.ae/scim2/ServiceProviderConfig\n    http_status: 200\n    content_type: application/scim+json\n    readable_without_auth:\n      - https://eisprod.uaeu.ac.ae/scim2/ServiceProviderConfig\n      - https://eisprod.uaeu.ac.ae/scim2/ResourceTypes\n    auth_required:\n      - https://eisprod.uaeu.ac.ae/scim2/Schemas\n      - https://eisprod.uaeu.ac.ae/scim2/Users\n    authentication_schemes: [ oauthbearertoken, httpbasic ]\n    notes: >-\n      SCIM 2.0 provisioning surface. ServiceProviderConfig and ResourceTypes\n      return\
  \ 200 unauthenticated; Schemas returns 401. documentationUri in the\n      served config is the WSO2 product default (example.com), not a UAEU\n      document.\nnot_found:\n  - what: developer portal / API key self-service\n    evidence: no host found under uaeu.ac.ae; no reference in sitemap.xml\n  - what: OAuth application registration for third parties\n    evidence: DCR endpoint advertised but no public onboarding documentation\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/united-arab-emirates-university/refs/heads/main/authentication/united-arab-emirates-university-authentication.yml
summary_line: 0 schemes
tags:
- University
- Higher Education
- Education
- United Arab Emirates
- Middle East
- Public Research University
- Identity Federation
- Research Repository
- Open Data
- OAI-PMH
- SCIM
- SAML
---
