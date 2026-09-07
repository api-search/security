---
anonymous_access: false
api_key_in: []
api_specs:
- filename: bnsf-trace-openapi.yml
  format: yaml
  label: BNSF Tracing API
  slug: bnsf-tracing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bnsf/refs/heads/main/openapi/bnsf-trace-openapi.yml
- filename: bnsf-intermodal-hub-operations-openapi.yml
  format: yaml
  label: BNSF Intermodal Hub Operations API
  slug: bnsf-hub-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bnsf/refs/heads/main/openapi/bnsf-intermodal-hub-operations-openapi.yml
- filename: bnsf-automotive-hub-operations-openapi.yml
  format: yaml
  label: BNSF Automotive Hub Operations API
  slug: bnsf-automotive-hub-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bnsf/refs/heads/main/openapi/bnsf-automotive-hub-operations-openapi.yml
- filename: bnsf-prices-openapi.yml
  format: yaml
  label: BNSF Prices and Rates API
  slug: bnsf-pricing-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bnsf/refs/heads/main/openapi/bnsf-prices-openapi.yml
- filename: bnsf-schedules-openapi.yml
  format: yaml
  label: BNSF Schedules API
  slug: bnsf-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bnsf/refs/heads/main/openapi/bnsf-schedules-openapi.yml
- filename: bnsf-waybill-openapi.yml
  format: yaml
  label: BNSF Waybill Management API
  slug: bnsf-waybill-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bnsf/refs/heads/main/openapi/bnsf-waybill-openapi.yml
- filename: bnsf-reference-files-openapi.yml
  format: yaml
  label: BNSF Reference Files API
  slug: bnsf-reference-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bnsf/refs/heads/main/openapi/bnsf-reference-files-openapi.yml
- filename: bnsf-diagnostics-openapi.yml
  format: yaml
  label: BNSF Diagnostics API
  slug: bnsf-diagnostics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bnsf/refs/heads/main/openapi/bnsf-diagnostics-openapi.yml
auth_types:
- mutualTLS
description: 'The BNSF Customer API has exactly one authentication mechanism: certificate-based mutual TLS. There is no API key, no bearer token, no OAuth and no OpenID Connect anywhere on the surface. Identity is the client certificate itself, and authorisation — which shipments a caller may see — is bound to the company on that certificate through the BNSF.com profile it is registered against.'
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Bnsf Authentication
name_suffix: Authentication
oauth_flows: []
overview: BNSF secures its APIs with mutualTLS across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: BNSF
provider_slug: bnsf
scheme_count: 2
schemes:
- accepted_cas_named_by_provider:
  - Entrust
  - Sectigo
  - GoDaddy
  - Comodo
  - DigiCert
  certificate_requirements:
  - x509 PEM format, unencrypted for use in Postman
  - issued by a recognised public Certificate Authority; Domain Validation, Organization Validation, Extended Validation and S/MIME (email) certificates are all accepted
  - self-signed and private certificates are NOT accepted
  - certificates from Let's Encrypt, webCARES and Cloudflare.com are explicitly NOT accepted
  - effective period no longer than 36 months
  - Organization Name must match the company name on the BNSF.com profile
  - Common Name must be the domain name (TLS/SSL) or the email address (S/MIME)
  - the domain of the registering email address must match the certificate's domain
  - Extended Key Usage must include Client Authentication (OID 1.3.6.1.5.5.7.3.2)
  description: Two-way TLS. The client validates BNSF's server certificate and BNSF validates the client's. Applies to every operation on every service.
  name: MutualTLS
  sources:
  - https://www.bnsf.com/ship-with-bnsf/support-services/customer-api/getting-started/
  transport: TLS client certificate on port 6443
  type: mutualTLS
- description: A second authorisation tier layered on the same client certificate. Operations flagged as Restricted Services require the certificate to be separately approved for that service; an unapproved caller receives HTTP 403 with "Insufficient privileges". Restricted Services are available in the Production environment only, and BNSF requires at least one unrestricted service to be working before it will move a caller to Production.
  name: Restricted
  operations_declared_restricted_in_the_specs: 27
  operations_total: 59
  request_channel: Customer Portal "Message Us" — Business Segment, Web Support, Reason "Application Programming Interface (API)", Sub Reason "Restricted Services"
  restricted_share: 46%
  sources:
  - https://www.bnsf.com/ship-with-bnsf/support-services/customer-api/support/
  - https://www.bnsf.com/ship-with-bnsf/support-services/customer-api/developers-console/
  type: mutualTLS
slug: bnsf-authentication
source_filename: bnsf-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: searched\nsource: https://www.bnsf.com/ship-with-bnsf/support-services/customer-api/getting-started/\ndocs:\n- https://www.bnsf.com/ship-with-bnsf/support-services/customer-api/getting-started/\n- https://www.bnsf.com/ship-with-bnsf/support-services/customer-api/support/\n- https://www.bnsf.com/ship-with-bnsf/support-services/customer-api/registration/\ndescription: >-\n  The BNSF Customer API has exactly one authentication mechanism: certificate-based mutual TLS.\n  There is no API key, no bearer token, no OAuth and no OpenID Connect anywhere on the surface.\n  Identity is the client certificate itself, and authorisation — which shipments a caller may see —\n  is bound to the company on that certificate through the BNSF.com profile it is registered against.\nsummary:\n  types:\n  - mutualTLS\n  api_key: false\n  oauth2: false\n  openid_connect: false\n  http_bearer: false\n  tiers: 2\nschemes:\n- name: MutualTLS\n  type: mutualTLS\n  transport:\
  \ TLS client certificate on port 6443\n  description: >-\n    Two-way TLS. The client validates BNSF's server certificate and BNSF validates the client's.\n    Applies to every operation on every service.\n  certificate_requirements:\n  - x509 PEM format, unencrypted for use in Postman\n  - issued by a recognised public Certificate Authority; Domain Validation, Organization Validation,\n    Extended Validation and S/MIME (email) certificates are all accepted\n  - self-signed and private certificates are NOT accepted\n  - certificates from Let's Encrypt, webCARES and Cloudflare.com are explicitly NOT accepted\n  - effective period no longer than 36 months\n  - Organization Name must match the company name on the BNSF.com profile\n  - Common Name must be the domain name (TLS/SSL) or the email address (S/MIME)\n  - the domain of the registering email address must match the certificate's domain\n  - Extended Key Usage must include Client Authentication (OID 1.3.6.1.5.5.7.3.2)\n  accepted_cas_named_by_provider:\n\
  \  - Entrust\n  - Sectigo\n  - GoDaddy\n  - Comodo\n  - DigiCert\n  sources:\n  - https://www.bnsf.com/ship-with-bnsf/support-services/customer-api/getting-started/\n- name: Restricted\n  type: mutualTLS\n  description: >-\n    A second authorisation tier layered on the same client certificate. Operations flagged as\n    Restricted Services require the certificate to be separately approved for that service; an\n    unapproved caller receives HTTP 403 with \"Insufficient privileges\". Restricted Services are\n    available in the Production environment only, and BNSF requires at least one unrestricted\n    service to be working before it will move a caller to Production.\n  request_channel: Customer Portal \"Message Us\" — Business Segment, Web Support, Reason \"Application\n    Programming Interface (API)\", Sub Reason \"Restricted Services\"\n  operations_declared_restricted_in_the_specs: 27\n  operations_total: 59\n  restricted_share: 46%\n  sources:\n  - https://www.bnsf.com/ship-with-bnsf/support-services/customer-api/support/\n\
  \  - https://www.bnsf.com/ship-with-bnsf/support-services/customer-api/developers-console/\nauthorization_model:\n  subject: the company named on the client certificate, bound to a BNSF.com User ID\n  data_scope: >-\n    A caller only receives data for equipment whose waybill names their company. A company not on\n    the waybill sees an empty result, not an error. Third-party visibility is granted either by\n    being added to the waybill in the ZS monitoring role at waybill creation, or by a Letter of\n    Authorization (LOA) issued by the shipper through the BNSF Customer Portal.\n  sources:\n  - https://www.bnsf.com/ship-with-bnsf/support-services/customer-api/support/\nonboarding:\n  self_service: false\n  steps:\n  - Obtain a BNSF.com User ID for an individual in the organisation (one per company is normally enough).\n  - Obtain a conforming client certificate from an accepted Certificate Authority.\n  - Register the certificate through the Customer Portal \"Message Us\" box — Business\
  \ Segment,\n    Web Support, Reason \"Application Programming Interface (API)\", Sub Reason \"API Registration\".\n  - Wait for BNSF to complete configuration; the provider states this takes up to five business days\n    and is confirmed by email.\n  provisioning_sla_days: 5\n  source: https://www.bnsf.com/ship-with-bnsf/support-services/customer-api/registration/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bnsf/refs/heads/main/authentication/bnsf-authentication.yml
summary_line: mutualTLS · 2 schemes
tags:
- Freight
- Railroad
- Shipping
- Trains
- Intermodal
- Logistics
- Supply Chain
- Transportation
---
