---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Ens Lyon Authentication
name_suffix: Authentication
oauth_flows: []
overview: École Normale Supérieure de Lyon declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: École Normale Supérieure de Lyon
provider_slug: ens-lyon
scheme_count: 0
schemes: []
slug: ens-lyon-authentication
source_filename: ens-lyon-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "---\n# How access to École Normale Supérieure de Lyon's programmable surfaces is actually established.\n# NOT an OAuth developer program: ENS de Lyon publishes no API keys and no client registration.\nname: École Normale Supérieure de Lyon — authentication and federated identity\nslug: ens-lyon\ngenerated: '2026-09-01'\nmethod: probed\nsource: https://idp.ens-lyon.fr/idp/shibboleth\nsummary: >-\n  ENS de Lyon has no public developer authentication surface — no API key issuance, no OAuth\n  client registration, no documented token endpoint for third parties, no developer portal.\n  What it does operate is institutional federated identity for its own members, in three\n  stacks, all of which answer unauthenticated metadata or protocol requests even though every\n  useful operation behind them requires an ENS de Lyon account.\nmechanisms:\n  - id: shibboleth-idp\n    type: saml2-idp\n    operator: institution\n    entity_id: https://idp.ens-lyon.fr/idp/shibboleth\n    metadata_url:\
  \ https://idp.ens-lyon.fr/idp/shibboleth\n    authoritative_metadata_url: https://mdq.federation.renater.fr/fer/entities/https%3A%2F%2Fidp.ens-lyon.fr%2Fidp%2Fshibboleth\n    scopes_asserted:\n      - ens-lyon.fr\n    protocols:\n      - urn:mace:shibboleth:1.0\n      - urn:oasis:names:tc:SAML:1.1:protocol\n      - urn:oasis:names:tc:SAML:2.0:protocol\n    sso_endpoints:\n      - binding: urn:mace:shibboleth:1.0:profiles:AuthnRequest\n        location: https://idp.ens-lyon.fr/idp/profile/Shibboleth/SSO\n      - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST\n        location: https://idp.ens-lyon.fr/idp/profile/SAML2/POST/SSO\n      - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect\n        location: https://idp.ens-lyon.fr/idp/profile/SAML2/Redirect/SSO\n    federation: Fédération Éducation-Recherche (RENATER), exported to eduGAIN\n    registration_authority: https://federation.renater.fr/\n    entity_categories:\n      - http://refeds.org/category/research-and-scholarship\n\
  \    technical_contact: admin-system@ens-lyon.fr\n    host_resolution: idp.ens-lyon.fr -> lxc-idp.ens-lyon.fr -> 140.77.167.96 (ENS de Lyon allocation)\n    audience: ENS de Lyon staff, students and federated service providers\n    public_client_registration: false\n    probed:\n      status: 200\n      content_type: application/xml;charset=UTF-8\n      bytes: 12129\n      date: '2026-09-01'\n    note: >-\n      The copy served from idp.ens-lyon.fr is the Shibboleth stock template — it still carries\n      the \"This is example metadata only\" comment and the commented-out mdui block. It is\n      nonetheless a valid EntityDescriptor with the real entityID, the real ens-lyon.fr scope\n      and the real signing key. The signed, curated metadata is RENATER's, recorded below.\n    method: probed\n    source: https://idp.ens-lyon.fr/idp/shibboleth\n  - id: renater-fer-entity\n    type: federation-metadata\n    operator: federation\n    mdq_base: https://mdq.federation.renater.fr/\n    namespaces_present:\n\
  \      - fer\n      - edugain\n      - fer+edugain\n    entity_id: https://idp.ens-lyon.fr/idp/shibboleth\n    required_accept_header: application/samlmetadata+xml\n    aggregate_url: https://metadata.federation.renater.fr/renater/main/main-idps-renater-metadata.xml\n    organization_name: Ecole Normale Supérieure de Lyon\n    display_name:\n      fr: ENS de Lyon\n      en: ENS de Lyon\n    probed:\n      status: 200\n      bytes_fer: 9123\n      bytes_edugain: 9541\n      aggregate_entities: 344\n      aggregate_contains_ens_lyon: true\n      date: '2026-09-01'\n    note: >-\n      A federation is shared by definition; recording it is not a misattribution. The IdP the\n      metadata describes is ENS de Lyon's own, and RENATER is the registration authority.\n    method: probed\n    source: https://mdq.federation.renater.fr/fer/entities/https%3A%2F%2Fidp.ens-lyon.fr%2Fidp%2Fshibboleth\n  - id: entra-id-tenant\n    type: oidc-and-saml2\n    operator: federation\n    tenant_id: c30cf67d-aee4-44f6-8f1b-12f4935b7d2c\n\
  \    tenant_region_scope: EU\n    issuer: https://login.microsoftonline.com/c30cf67d-aee4-44f6-8f1b-12f4935b7d2c/v2.0\n    discovery_url: https://login.microsoftonline.com/ens-lyon.fr/v2.0/.well-known/openid-configuration\n    authorization_endpoint: https://login.microsoftonline.com/c30cf67d-aee4-44f6-8f1b-12f4935b7d2c/oauth2/v2.0/authorize\n    token_endpoint: https://login.microsoftonline.com/c30cf67d-aee4-44f6-8f1b-12f4935b7d2c/oauth2/v2.0/token\n    jwks_uri: https://login.microsoftonline.com/c30cf67d-aee4-44f6-8f1b-12f4935b7d2c/discovery/v2.0/keys\n    saml_metadata_url: https://login.microsoftonline.com/c30cf67d-aee4-44f6-8f1b-12f4935b7d2c/federationmetadata/2007-06/federationmetadata.xml\n    audience: ENS de Lyon accounts on Microsoft 365 and SAML-integrated internal systems\n    public_client_registration: false\n    probed:\n      oidc_status: 200\n      oidc_bytes: 1964\n      saml_status: 200\n      saml_bytes: 28441\n      date: '2026-09-01'\n    note: >-\n      login.microsoftonline.com\
  \ is Microsoft's host and Microsoft's contract. The TENANT is\n      ENS de Lyon's, resolved from the ens-lyon.fr domain hint, which is why this is recorded\n      as federation and no Microsoft specification is saved under this institution.\n    method: probed\n    source: https://login.microsoftonline.com/ens-lyon.fr/v2.0/.well-known/openid-configuration\n  - id: cas-sso\n    type: cas3\n    operator: institution\n    base_url: https://cas.ens-lyon.fr/cas/\n    login_endpoint: https://cas.ens-lyon.fr/cas/login\n    validate_endpoint: https://cas.ens-lyon.fr/cas/p3/serviceValidate\n    host_resolution: cas.ens-lyon.fr -> 140.77.51.3 (ENS de Lyon allocation)\n    audience: ENS de Lyon accounts on internally integrated web services\n    public_client_registration: false\n    probed:\n      status: 200\n      bytes: 167\n      response: >-\n        <cas:serviceResponse xmlns:cas='http://www.yale.edu/tp/cas'><cas:authenticationFailure\n        code=\"INVALID_REQUEST\"/></cas:serviceResponse>\n\
  \      date: '2026-09-01'\n    note: >-\n      Apereo CAS on ENS de Lyon's own host. The protocol surface is real and probeable; there\n      is no third-party client registration and no published integration guide, so it is\n      institutional plumbing rather than a developer program.\n    method: probed\n    source: https://cas.ens-lyon.fr/cas/p3/serviceValidate\ntenant_access:\n  - id: hal-deposit\n    platform: HAL (CCSD / CNRS)\n    operator: tenant\n    note: >-\n      Depositing into the ens-lyon collection uses HAL's own credentials and HAL's SWORD\n      endpoint at api.archives-ouvertes.fr/sword/. That endpoint is generic — it carries no\n      ENS de Lyon scope — so it is HAL's contract, not ENS de Lyon's, and it is not recorded\n      as one of this institution's APIs. Read access to the ens-lyon scope is unauthenticated.\n    method: probed\n    source: https://api.archives-ouvertes.fr/docs/sword\nabsent:\n  - api_keys: not issued\n  - oauth_client_registration: none published\n\
  \  - developer_portal: none; api.ens-lyon.fr and developer.ens-lyon.fr do not resolve\n  - scim_provisioning: not publicly exposed\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ens-lyon/refs/heads/main/authentication/ens-lyon-authentication.yml
summary_line: 0 schemes
tags:
- University
- Higher Education
- Education
- France
- Grande École
- Identity Federation
- Shibboleth
- SAML
- Research Repository
- Open Access
- OAI-PMH
- Research Computing
---
