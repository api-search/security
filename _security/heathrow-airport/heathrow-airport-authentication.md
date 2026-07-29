---
api_key_in: []
auth_types:
- mutualTLS
- federated-sso
description: Heathrow runs a two-layer authentication model, and both layers are closed to anonymous callers. Human access to the developer portal is federated to Microsoft Entra ID (Azure Active Directory) and only issued after a manual enrolment conversation with Heathrow. Machine access to the runtime gateway at api.heathrow.com is gated by mutual TLS - the Azure Application Gateway terminates every anonymous request with "400 No required SSL certificate was sent" before routing, so a client certificate issued by Heathrow is a precondition to reaching any operation. No OpenAPI is published, so no securityScheme could be derived; this profile is taken from the provider's own public prose plus observed gateway behaviour.
kind: authentication
layout: security
method: searched
name: Heathrow Airport Authentication
name_suffix: Authentication
oauth_flows: []
overview: Heathrow Airport secures its APIs with mutualTLS and federated-sso across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Heathrow Airport
provider_slug: heathrow-airport
scheme_count: 2
schemes:
- discovery_document: null
  evidence: https://developer.heathrow.com/signin - "Sign in using your Azure Active Directory credentials." No local-account option is offered. The portal is Azure API Management (config.json names the APIM instance apim-halcomcommon-prod-westeu-001 behind https://apimgmt.lhr.aero).
  layer: developer-portal (human)
  name: microsoft-entra-id
  note: No tenant-specific /.well-known/openid-configuration is published on any Heathrow host, so the issuer, supported flows and scopes are not externally discoverable.
  provider: Microsoft Entra ID (Azure Active Directory)
  type: openIdConnect
- evidence: Every path under https://api.heathrow.com returns HTTP 400 from Microsoft-Azure-Application-Gateway/v2 with the body "400 No required SSL certificate was sent". The same rejection occurs at https://apimgmt.lhr.aero/ root. The developer portal's own sitemap lists /documentation/requesting-a-client-certificate, confirming Heathrow issues client certificates - though that page itself returns 404.
  host: https://api.heathrow.com
  layer: api-gateway (machine)
  name: mutual-tls-client-certificate
  note: The certificate request process is documented in the sitemap but the document does not resolve; obtaining a certificate runs through the enrolment channel below.
  type: mutualTLS
slug: heathrow-airport-authentication
source_filename: heathrow-airport-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-28'\nmethod: searched\nsource: >-\n  https://developer.heathrow.com/how-it-works, https://developer.heathrow.com/signin,\n  https://developer.heathrow.com/config.json, and live probes of\n  https://api.heathrow.com/ and https://apimgmt.lhr.aero/ on 2026-07-28.\ndocs: https://developer.heathrow.com/how-it-works\ndescription: >-\n  Heathrow runs a two-layer authentication model, and both layers are closed to\n  anonymous callers. Human access to the developer portal is federated to\n  Microsoft Entra ID (Azure Active Directory) and only issued after a manual\n  enrolment conversation with Heathrow. Machine access to the runtime gateway at\n  api.heathrow.com is gated by mutual TLS - the Azure Application Gateway\n  terminates every anonymous request with \"400 No required SSL certificate was\n  sent\" before routing, so a client certificate issued by Heathrow is a\n  precondition to reaching any operation. No OpenAPI is published, so no\n  securityScheme could\
  \ be derived; this profile is taken from the provider's own\n  public prose plus observed gateway behaviour.\nsummary:\n  types: [mutualTLS, federated-sso]\n  api_key_in: []\n  oauth2_flows: []\n  derived_from_openapi: false\n  anonymous_access: false\n  self_service_credentials: false\nschemes:\n  - name: microsoft-entra-id\n    type: openIdConnect\n    layer: developer-portal (human)\n    provider: Microsoft Entra ID (Azure Active Directory)\n    discovery_document: null\n    evidence: >-\n      https://developer.heathrow.com/signin - \"Sign in using your Azure Active\n      Directory credentials.\" No local-account option is offered. The portal is\n      Azure API Management (config.json names the APIM instance\n      apim-halcomcommon-prod-westeu-001 behind https://apimgmt.lhr.aero).\n    note: >-\n      No tenant-specific /.well-known/openid-configuration is published on any\n      Heathrow host, so the issuer, supported flows and scopes are not\n      externally discoverable.\n \
  \ - name: mutual-tls-client-certificate\n    type: mutualTLS\n    layer: api-gateway (machine)\n    host: https://api.heathrow.com\n    evidence: >-\n      Every path under https://api.heathrow.com returns HTTP 400 from\n      Microsoft-Azure-Application-Gateway/v2 with the body \"400 No required SSL\n      certificate was sent\". The same rejection occurs at\n      https://apimgmt.lhr.aero/ root. The developer portal's own sitemap lists\n      /documentation/requesting-a-client-certificate, confirming Heathrow issues\n      client certificates - though that page itself returns 404.\n    note: >-\n      The certificate request process is documented in the sitemap but the\n      document does not resolve; obtaining a certificate runs through the\n      enrolment channel below.\nonboarding:\n  model: application-approval\n  steps:\n    - Contact Heathrow at support@heathrow.com or 08443351801 and state what type of user you are and why you want to use the APIs.\n    - Heathrow returns enrolment\
  \ details and runs an approval process.\n    - On approval an account is provisioned and access is via Microsoft Active Directory.\n    - Product entitlement is chosen during enrolment.\n  verbatim: >-\n    \"In order to get the access to our APIs you need to get a personal account\n    or an account for you team, for security and privacy reasons before we grant\n    you access to the APIs, we need to know what type of user you are and why\n    you want to use the APIs. ... Once you contacted us we'll give you the\n    details to start our enrolling process, once you account is ready you'll be\n    able to access using the Microsoft active directory and you'll have\n    unlimited access to the product you choose during the enrolment procedure.\"\n  source: https://developer.heathrow.com/how-it-works\n  contact:\n    email: support@heathrow.com\n    phone: '08443351801'\nnot_observed:\n  - api_key: >-\n      Azure API Management normally issues per-subscription keys\n      (Ocp-Apim-Subscription-Key),\
  \ and the portal's /products page is the\n      standard APIM subscription surface - but the products list renders empty\n      to anonymous visitors and Heathrow documents no key header publicly, so no\n      api-key scheme is asserted here.\n  - oauth2: >-\n      A /signup-oauth page exists in the portal sitemap (HTTP 200) but exposes no\n      authorization or token endpoint, and no OAuth metadata is published.\n  - scopes: >-\n      No scope or permission reference is published; scopes/ is intentionally\n      absent for this provider.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/heathrow-airport/refs/heads/main/authentication/heathrow-airport-authentication.yml
summary_line: mutualTLS/federated-sso · 2 schemes
tags:
- Travel
- United Kingdom
- Airports
- Aviation
- Airport Infrastructure
- Flight Information
- Transportation
- Passenger Experience
---
