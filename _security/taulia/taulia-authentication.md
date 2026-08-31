---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Taulia Authentication
name_suffix: Authentication
oauth_flows: []
overview: Taulia declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Taulia
provider_slug: taulia
scheme_count: 4
schemes:
- applies_to: Buyer integration API (SAP S/4HANA Cloud Public Edition activation)
  detail: The customer creates an OpenID Connect application in SAP Cloud Identity Services (IAS), configures a client secret for API authentication, and adds a self-defined `aud` attribute to single sign-on. The token is then trusted by SAP Taulia through a token setup registered in the Taulia platform under Settings > Integrations > Setup Token.
  documented: true
  id: oauth2-jwt-bearer-ias
  note: The audience string `extapi-buyer-integration` is the only publicly published identifier of SAP Taulia's external buyer integration API.
  parameters:
    audience: extapi-buyer-integration
    issuer: the customer's SAP IAS tenant URL (e.g. https://<tenant>.accounts400.ondemand.com)
    jwks_url: the IAS certificate URL — the customer's https://<IAS INSTANCE URL>/.well-known/openid-configuration or its /oauth2/certs endpoint
    subject: the Client ID generated in IAS
  source: https://support.taulia.com/article/Easy-Guide-to-Activating-SAP-Taulia-with-S-4HANA-Cloud-Public-Edition
  subtype: jwt-bearer-trust
  type: oauth2
- applies_to: Taulia Buyer API and Taulia Supplier API (direct REST integration)
  detail: The Description of Software Services states that the direct API integration follows RESTful principles with resource-oriented URLs, JSON request and response bodies, HTTP verbs and HTTP status codes for errors, and that authentication uses an assigned API key.
  documented: true
  id: api-key-secret
  note: The DSS does not publish the header name, the signing algorithm, or a key prefix. Key issuance is handled by SAP Taulia during customer onboarding, not through self-service.
  parameters:
    header: unknown
    key_prefix: unknown
  source: https://taulia.com/dss/
  type: apiKey
- applies_to: Taulia platform web portal (human sign-in, not API)
  detail: SAML 2.0 single sign-on is supported with response signing; assertion encryption is not supported.
  documented: true
  id: saml2-sso
  source: https://taulia.com/dss/
  type: federated-sso
- applies_to: Taulia platform web portal (human sign-in, not API)
  detail: Two-factor authentication is available and can be mandated for an account.
  documented: true
  id: mfa
  source: https://taulia.com/dss/
  type: two-factor
slug: taulia-authentication
source_filename: taulia-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: searched\nsource: https://support.taulia.com/article/Easy-Guide-to-Activating-SAP-Taulia-with-S-4HANA-Cloud-Public-Edition + https://taulia.com/dss/\nnote: >-\n  DERIVED FROM DOCS ONLY. SAP Taulia publishes no OpenAPI, so there are no securitySchemes to\n  read; every scheme below is transcribed from SAP Taulia's own published documentation and is\n  marked with the page it came from. Nothing here was inferred from a spec.\ndocs:\n- https://support.taulia.com/article/Easy-Guide-to-Activating-SAP-Taulia-with-S-4HANA-Cloud-Public-Edition\n- https://taulia.com/dss/\n- https://support.taulia.com/technical-resources/connection-type\nschemes:\n- id: oauth2-jwt-bearer-ias\n  type: oauth2\n  subtype: jwt-bearer-trust\n  applies_to: Buyer integration API (SAP S/4HANA Cloud Public Edition activation)\n  documented: true\n  source: https://support.taulia.com/article/Easy-Guide-to-Activating-SAP-Taulia-with-S-4HANA-Cloud-Public-Edition\n  detail: >-\n \
  \   The customer creates an OpenID Connect application in SAP Cloud Identity Services (IAS),\n    configures a client secret for API authentication, and adds a self-defined `aud` attribute to\n    single sign-on. The token is then trusted by SAP Taulia through a token setup registered in\n    the Taulia platform under Settings > Integrations > Setup Token.\n  parameters:\n    audience: extapi-buyer-integration\n    issuer: the customer's SAP IAS tenant URL (e.g. https://<tenant>.accounts400.ondemand.com)\n    jwks_url: >-\n      the IAS certificate URL — the customer's\n      https://<IAS INSTANCE URL>/.well-known/openid-configuration or its /oauth2/certs endpoint\n    subject: the Client ID generated in IAS\n  note: >-\n    The audience string `extapi-buyer-integration` is the only publicly published identifier of\n    SAP Taulia's external buyer integration API.\n- id: api-key-secret\n  type: apiKey\n  applies_to: Taulia Buyer API and Taulia Supplier API (direct REST integration)\n \
  \ documented: true\n  source: https://taulia.com/dss/\n  detail: >-\n    The Description of Software Services states that the direct API integration follows RESTful\n    principles with resource-oriented URLs, JSON request and response bodies, HTTP verbs and HTTP\n    status codes for errors, and that authentication uses an assigned API key.\n  parameters:\n    header: unknown\n    key_prefix: unknown\n  note: >-\n    The DSS does not publish the header name, the signing algorithm, or a key prefix. Key issuance\n    is handled by SAP Taulia during customer onboarding, not through self-service.\n- id: saml2-sso\n  type: federated-sso\n  applies_to: Taulia platform web portal (human sign-in, not API)\n  documented: true\n  source: https://taulia.com/dss/\n  detail: >-\n    SAML 2.0 single sign-on is supported with response signing; assertion encryption is not\n    supported.\n- id: mfa\n  type: two-factor\n  applies_to: Taulia platform web portal (human sign-in, not API)\n  documented: true\n\
  \  source: https://taulia.com/dss/\n  detail: Two-factor authentication is available and can be mandated for an account.\nnot_the_api_authorization_server:\n- url: https://support.taulia.com/.well-known/openid-configuration\n  status: 200\n  issuer: https://support.taulia.com/vforcesite\n  note: >-\n    This 200 is the stock Salesforce Experience Cloud OIDC discovery document for the SAP Taulia\n    support community. Its scopes are Salesforce platform scopes (api, web, chatter_api,\n    cdp_*_api, wave_api …), not Taulia API scopes. It is recorded so a later pass does not mistake\n    it for the Taulia API authorization server; nothing was derived from it and no scopes/\n    artifact was written from it.\ngaps:\n- No public authentication reference page with header names, token lifetimes, or error responses.\n- No self-service key issuance; credentials are provisioned during onboarding.\n- No published OAuth scope list for the Buyer or Supplier API.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/taulia/refs/heads/main/authentication/taulia-authentication.yml
summary_line: 4 schemes
tags:
- Company
- Working Capital
- Supply Chain Finance
- Dynamic Discounting
- Accounts Payable
- Accounts Receivable
- Invoicing
- Payments
- Procurement
- Financial-Services
- ERP Integration
- SAP
---
