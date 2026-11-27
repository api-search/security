---
anonymous_access: false
api_key_in: []
api_specs:
- filename: envestnet-account-token-api-openapi.yml
  format: yaml
  label: Envestnet Account Token API
  slug: envestnet-account-token-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/envestnet/openapi/envestnet-account-token-api-openapi.yml
- filename: envestnet-accounts-api-openapi.yml
  format: yaml
  label: Envestnet Accounts API
  slug: envestnet-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/envestnet/openapi/envestnet-accounts-api-openapi.yml
- filename: envestnet-associated-details-api-openapi.yml
  format: yaml
  label: Envestnet Associated Details API
  slug: envestnet-associated-details-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/envestnet/openapi/envestnet-associated-details-api-openapi.yml
- filename: envestnet-auth-api-openapi.yml
  format: yaml
  label: Envestnet Auth API
  slug: envestnet-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/envestnet/openapi/envestnet-auth-api-openapi.yml
- filename: envestnet-configs-api-openapi.yml
  format: yaml
  label: Envestnet Configs API
  slug: envestnet-configs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/envestnet/openapi/envestnet-configs-api-openapi.yml
- filename: envestnet-consents-api-openapi.yml
  format: yaml
  label: Envestnet Consents API
  slug: envestnet-consents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/envestnet/openapi/envestnet-consents-api-openapi.yml
- filename: envestnet-creditacceleratorfile-api-openapi.yml
  format: yaml
  label: Envestnet CreditAcceleratorFile API
  slug: envestnet-creditacceleratorfile-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/envestnet/openapi/envestnet-creditacceleratorfile-api-openapi.yml
- filename: envestnet-customer-api-openapi.yml
  format: yaml
  label: Envestnet Customer API
  slug: envestnet-customer-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/envestnet/openapi/envestnet-customer-api-openapi.yml
- filename: envestnet-dataextracts-api-openapi.yml
  format: yaml
  label: Envestnet DataExtracts API
  slug: envestnet-dataextracts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/envestnet/openapi/envestnet-dataextracts-api-openapi.yml
- filename: envestnet-derived-api-openapi.yml
  format: yaml
  label: Envestnet Derived API
  slug: envestnet-derived-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/envestnet/openapi/envestnet-derived-api-openapi.yml
- filename: envestnet-documents-api-openapi.yml
  format: yaml
  label: Envestnet Documents API
  slug: envestnet-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/envestnet/openapi/envestnet-documents-api-openapi.yml
- filename: envestnet-holdings-api-openapi.yml
  format: yaml
  label: Envestnet Holdings API
  slug: envestnet-holdings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/envestnet/openapi/envestnet-holdings-api-openapi.yml
- filename: envestnet-payment-processor-api-openapi.yml
  format: yaml
  label: Envestnet Payment Processor API
  slug: envestnet-payment-processor-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/envestnet/openapi/envestnet-payment-processor-api-openapi.yml
- filename: envestnet-providers-api-openapi.yml
  format: yaml
  label: Envestnet Providers API
  slug: envestnet-providers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/envestnet/openapi/envestnet-providers-api-openapi.yml
- filename: envestnet-statements-api-openapi.yml
  format: yaml
  label: Envestnet Statements API
  slug: envestnet-statements-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/envestnet/openapi/envestnet-statements-api-openapi.yml
- filename: envestnet-transactions-api-openapi.yml
  format: yaml
  label: Envestnet Transactions API
  slug: envestnet-transactions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/envestnet/openapi/envestnet-transactions-api-openapi.yml
- filename: envestnet-user-api-openapi.yml
  format: yaml
  label: Envestnet User API
  slug: envestnet-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/envestnet/openapi/envestnet-user-api-openapi.yml
- filename: envestnet-verification-api-openapi.yml
  format: yaml
  label: Envestnet Verification API
  slug: envestnet-verification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/envestnet/openapi/envestnet-verification-api-openapi.yml
- filename: envestnet-verify-account-api-openapi.yml
  format: yaml
  label: Envestnet Verify Account API
  slug: envestnet-verify-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/envestnet/openapi/envestnet-verify-account-api-openapi.yml
- filename: envestnet-view-api-openapi.yml
  format: yaml
  label: Envestnet View API
  slug: envestnet-view-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/envestnet/openapi/envestnet-view-api-openapi.yml
- filename: envestnet-provider-accounts-api-openapi.yml
  format: yaml
  label: Envestnet Provider Accounts API
  slug: envestnet-provider-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/envestnet/openapi/envestnet-provider-accounts-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Envestnet Authentication
name_suffix: Authentication
oauth_flows: []
overview: Envestnet declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Envestnet
provider_slug: envestnet
scheme_count: 1
schemes:
- details:
  - SAML responses must be encrypted using Envestnets SSO certificate; partners provide a UAT signing certificate (Base64 .cer, .pem, or metadata), and Envestnet provides the encryption certificate and ACS URL.
  - A firm code (included in the ACS URL) identifies the partner and is used to validate SAML responses against the correct signing certificate
  environments:
  - UAT
  - Production
  flow: IdP-initiated SAML 2.0
  name: Envestnet Enterprise single sign-on
  purpose: user SSO into Envestnet Enterprise (advisors, home office users, money managers, clients), not API calls
  quote: Envestnet Enterprise supports single sign-on (SSO) for advisors, home office users, money managers, and clients using IdP-initiated SAML 2.0.
  type: saml2
slug: envestnet-authentication
source_filename: envestnet-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: searched\nsource: https://developer.envestnet.com/products/envestnet/single-sign\ndocs: https://developer.envestnet.com/products/envestnet/single-sign\nnote: >-\n  The OpenAPI files in openapi/ declare no securitySchemes (derive-authentication.py found none). The API reference\n  and documentation pages on developer.envestnet.com (/products/*/docs, /docs/api) all return a portal login form, so\n  the API credential scheme is not publicly documented. The only public authentication documentation is the SAML 2.0\n  single sign-on page. Product pages refer to \"the authenticated user\" (Client Management) without naming the scheme.\nschemes:\n- type: saml2\n  name: Envestnet Enterprise single sign-on\n  flow: IdP-initiated SAML 2.0\n  purpose: user SSO into Envestnet Enterprise (advisors, home office users, money managers, clients), not API calls\n  quote: Envestnet Enterprise supports single sign-on (SSO) for advisors, home office users, money\
  \ managers, and clients using IdP-initiated SAML 2.0.\n  details:\n  - SAML responses must be encrypted using Envestnets SSO certificate; partners provide a UAT signing certificate (Base64 .cer, .pem, or metadata), and Envestnet provides the encryption certificate and ACS URL.\n  - A firm code (included in the ACS URL) identifies the partner and is used to validate SAML responses against the correct signing certificate\n  environments: [UAT, Production]\n"
source_yaml_url: https://artifacts.apis.io/envestnet/authentication/envestnet-authentication.yml
summary_line: 1 scheme
tags:
- Finance
- Wealth Management
- Open Banking
- Account Aggregation
- Wealth Technology
- Financial Planning
- Portfolio Management
- Financial Advisors
---
