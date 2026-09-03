---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Trinity College Dublin Authentication
name_suffix: Authentication
oauth_flows: []
overview: Trinity College Dublin declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Trinity College Dublin
provider_slug: trinity-college-dublin
scheme_count: 0
schemes: []
slug: trinity-college-dublin-authentication
source_filename: trinity-college-dublin-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "---\n# How access to Trinity College Dublin's programmable surfaces is actually established.\n# NOT an OAuth developer program: Trinity publishes no API keys and no client registration.\nname: Trinity College Dublin — authentication and federated identity\nslug: trinity-college-dublin\ngenerated: '2026-09-01'\nmethod: probed\nsource: https://idp.tcd.ie/idp/shibboleth\nsummary: >-\n  Trinity has no public developer authentication surface — no API key issuance, no OAuth client\n  registration, no documented token endpoint for third parties. What it does operate is\n  institutional federated identity for its own members, in two stacks that both answer\n  unauthenticated metadata requests.\nmechanisms:\n  - id: shibboleth-idp\n    type: saml2-idp\n    operator: institution\n    entity_id: https://idp.tcd.ie/idp/shibboleth\n    metadata_url: https://idp.tcd.ie/idp/shibboleth\n    scopes_asserted:\n      - tcd.ie\n      - blackboard.com\n    federation: Edugate (HEAnet), exported\
  \ to eduGAIN\n    audience: Trinity staff, students and federated service providers\n    public_client_registration: false\n    probed:\n      status: 200\n      content_type: application/xml\n      date: '2026-09-01'\n    method: probed\n    source: https://idp.tcd.ie/idp/shibboleth\n  - id: entra-id-tenant\n    type: oidc-and-saml2\n    operator: federation\n    tenant_id: d595be8d-b306-45f4-8064-9e5b82fbe52b\n    issuer: https://login.microsoftonline.com/d595be8d-b306-45f4-8064-9e5b82fbe52b/v2.0\n    discovery_url: https://login.microsoftonline.com/tcd.ie/v2.0/.well-known/openid-configuration\n    saml_metadata_url: https://login.microsoftonline.com/d595be8d-b306-45f4-8064-9e5b82fbe52b/federationmetadata/2007-06/federationmetadata.xml\n    authorization_endpoint: https://login.microsoftonline.com/d595be8d-b306-45f4-8064-9e5b82fbe52b/oauth2/v2.0/authorize\n    jwks_uri: https://login.microsoftonline.com/d595be8d-b306-45f4-8064-9e5b82fbe52b/discovery/v2.0/keys\n    audience: Trinity accounts\
  \ on Microsoft 365 and SAML-integrated internal systems (rss.tcd.ie observed redirecting here)\n    public_client_registration: false\n    note: >-\n      login.microsoftonline.com is Microsoft's host and Microsoft's contract. The TENANT is\n      Trinity's, resolved from the tcd.ie domain hint, which is why it is recorded as\n      `federation` rather than discarded as a vendor host.\n    probed:\n      status: 200\n      date: '2026-09-01'\n    method: probed\n    source: https://login.microsoftonline.com/tcd.ie/v2.0/.well-known/openid-configuration\nunauthenticated_surfaces:\n  - url: https://www.edepositireland.ie/server/oai/request?verb=Identify\n    detail: OAI-PMH harvesting is open; no credential required.\n  - url: https://www.tcd.ie/assets/xml/tcd-opensearch/tcd-opensearch.xml\n    detail: OpenSearch 1.1 description document; no credential required.\nblocked_surfaces:\n  - url: https://www.tara.tcd.ie/oai/request?verb=Identify\n    status: 403\n    detail: Cloudflare interstitial\
  \ (\"Just a moment...\"), not an authentication requirement.\n  - url: https://digitalcollections.tcd.ie/\n    status: 200\n    detail: >-\n      Soft-200 reCAPTCHA interstitial served by an F5 Distributed Cloud edge to every path,\n      including /robots.txt and IIIF manifest URLs. Not an authentication requirement.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trinity-college-dublin/refs/heads/main/authentication/trinity-college-dublin-authentication.yml
summary_line: 0 schemes
tags:
- University
- Higher Education
- Education
- Ireland
- Research Repository
- Identity Federation
- Library
- Open Access
- Digital Collections
- IIIF
- OAI-PMH
- Shibboleth
- DataCite
- Legal Deposit
---
