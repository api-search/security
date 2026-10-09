---
anonymous_access: false
api_key_in: []
api_specs:
- filename: groupe-bpce-aisp-api-openapi.yml
  format: yaml
  label: Groupe BPCE AISP API
  slug: groupe-bpce-aisp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groupe-bpce/refs/heads/main/openapi/groupe-bpce-aisp-api-openapi.yml
- filename: groupe-bpce-cbpii-api-openapi.yml
  format: yaml
  label: Groupe BPCE CBPII API
  slug: groupe-bpce-cbpii-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groupe-bpce/refs/heads/main/openapi/groupe-bpce-cbpii-api-openapi.yml
- filename: groupe-bpce-external-accounts-api-openapi.yml
  format: yaml
  label: Groupe BPCE External Accounts API
  slug: groupe-bpce-external-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groupe-bpce/refs/heads/main/openapi/groupe-bpce-external-accounts-api-openapi.yml
- filename: groupe-bpce-internal-accounts-api-openapi.yml
  format: yaml
  label: Groupe BPCE Internal Accounts API
  slug: groupe-bpce-internal-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groupe-bpce/refs/heads/main/openapi/groupe-bpce-internal-accounts-api-openapi.yml
- filename: groupe-bpce-pisp-api-openapi.yml
  format: yaml
  label: Groupe BPCE PISP API
  slug: groupe-bpce-pisp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groupe-bpce/refs/heads/main/openapi/groupe-bpce-pisp-api-openapi.yml
- filename: groupe-bpce-registration-api-openapi.yml
  format: yaml
  label: Groupe BPCE Registration API
  slug: groupe-bpce-registration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groupe-bpce/refs/heads/main/openapi/groupe-bpce-registration-api-openapi.yml
- filename: groupe-bpce-transfers-api-openapi.yml
  format: yaml
  label: Groupe BPCE Transfers API
  slug: groupe-bpce-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groupe-bpce/refs/heads/main/openapi/groupe-bpce-transfers-api-openapi.yml
auth_types:
- mutualTLS
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 5
method: searched
name: Groupe Bpce Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Groupe BPCE secures its APIs with mutualTLS and oauth2 across 5 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Groupe BPCE
provider_slug: groupe-bpce
scheme_count: 5
schemes:
- description: 'In order to access the PSU''s account information, the AISP needs to get either an authorization code grant or a Client Initiated Backchannel Authentication token.

    In order to post a funds confirmation request, the CBPII needs to get either an authorization code grant or a Client Initiated Backchannel Authentication token when registration of the account has not been previously processed.

    In order '
  flows:
  - authorizationUrl: /stet/psd2/oauth/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: /stet/psd2/oauth/token
  name: accessCode
  sources:
  - openapi/groupe-bpce-natixis-psd2-accounts-openapi.yml
  - openapi/groupe-bpce-natixis-wealth-management-psd2-accounts-openapi.yml
  - openapi/groupe-bpce-open-finance-transfer-openapi.yml
  - openapi/groupe-bpce-psd2-accounts-openapi.yml
  - openapi/groupe-bpce-psd2-funds-availability-openapi.yml
  - openapi/groupe-bpce-psd2-payments-openapi.yml
  type: oauth2
- description: 'In order to post, get or cancel a Payment or Transfer Request, the PISP needs to get a client credential OAUTH2 token.

    In order to confirm a Payment or Transfer Request, the PISP needs to get either an authorization code grant or a client credential OAUTH2 token.

    In order to post a funds confirmation request, the CBPII needs to get a client credential OAUTH2 token when registration of the account '
  flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: /stet/psd2/oauth/token
  name: clientCredentials
  sources:
  - openapi/groupe-bpce-psd2-funds-availability-openapi.yml
  - openapi/groupe-bpce-psd2-payments-openapi.yml
  type: oauth2
- description: '"Use of same TPP eIDAS certificate (QWAC) to be presented for mutual TLS authentication"; "TPP needs to use a TLS mutual authentication based on QWAC certificate with this POST /token method." Not declared as a securityScheme in the specs.'
  name: eidas-mtls
  sources:
  - https://apistore.groupebpce.com/api/account-information-services-3
  - https://apistore.groupebpce.com/api/psd2-registration
  type: mutualTLS
- description: PSD2 requests carry Signature and Digest headers (STET); the registration jwks must contain the QSEALC public key ("kty" RSA, "alg" RS256, "use" sig).
  name: http-signature-qsealc
  sources:
  - openapi/groupe-bpce-psd2-payments-openapi.yml
  - https://apistore.groupebpce.com/api/psd2-registration
  type: signature
- description: 'Registration API: generic client_id “PSD2_TPPRegister”, grant_type client_credentials, scope manageRegistration; returns a temporary access token; POST /register returns the client_id used in all PSD2 methods.'
  flows:
  - flow: clientCredentials
    tokenUrl: https://www.<codetab>.live.api.89C3.com/stet/psd2/oauth/token
  name: registration-client-credentials
  sources:
  - https://apistore.groupebpce.com/api/psd2-registration
  type: oauth2
slug: groupe-bpce-authentication
source_filename: groupe-bpce-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: searched\nsource: openapi/groupe-bpce-natixis-psd2-accounts-openapi.yml, openapi/groupe-bpce-natixis-wealth-management-psd2-accounts-openapi.yml,\n  openapi/groupe-bpce-open-finance-transfer-openapi.yml, openapi/groupe-bpce-psd2-accounts-openapi.yml, openapi/groupe-bpce-psd2-funds-availability-openapi.yml,\n  openapi/groupe-bpce-psd2-payments-openapi.yml, https://apistore.groupebpce.com/api/psd2-registration, https://apistore.groupebpce.com/api/account-information-services-3\nsummary:\n  types:\n  - mutualTLS\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: accessCode\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /stet/psd2/oauth/authorize\n    tokenUrl: /stet/psd2/oauth/token\n    scopes: 2\n  description: 'In order to access the PSU''s account information, the AISP needs to get either an authorization\n    code grant or a Client Initiated Backchannel Authentication\
  \ token.\n\n    In order to post a funds confirmation request, the CBPII needs to get either an authorization code grant or\n    a Client Initiated Backchannel Authentication token when registration of the account has not been previously\n    processed.\n\n    In order '\n  sources:\n  - openapi/groupe-bpce-natixis-psd2-accounts-openapi.yml\n  - openapi/groupe-bpce-natixis-wealth-management-psd2-accounts-openapi.yml\n  - openapi/groupe-bpce-open-finance-transfer-openapi.yml\n  - openapi/groupe-bpce-psd2-accounts-openapi.yml\n  - openapi/groupe-bpce-psd2-funds-availability-openapi.yml\n  - openapi/groupe-bpce-psd2-payments-openapi.yml\n- name: clientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /stet/psd2/oauth/token\n    scopes: 1\n  description: 'In order to post, get or cancel a Payment or Transfer Request, the PISP needs to get a client credential\n    OAUTH2 token.\n\n    In order to confirm a Payment or Transfer Request, the PISP needs to get either\
  \ an authorization code grant\n    or a client credential OAUTH2 token.\n\n    In order to post a funds confirmation request, the CBPII needs to get a client credential OAUTH2 token when\n    registration of the account '\n  sources:\n  - openapi/groupe-bpce-psd2-funds-availability-openapi.yml\n  - openapi/groupe-bpce-psd2-payments-openapi.yml\n- name: eidas-mtls\n  type: mutualTLS\n  description: '\"Use of same TPP eIDAS certificate (QWAC) to be presented for mutual TLS authentication\"; \"TPP needs\n    to use a TLS mutual authentication based on QWAC certificate with this POST /token method.\" Not declared as\n    a securityScheme in the specs.'\n  sources:\n  - https://apistore.groupebpce.com/api/account-information-services-3\n  - https://apistore.groupebpce.com/api/psd2-registration\n- name: http-signature-qsealc\n  type: signature\n  description: PSD2 requests carry Signature and Digest headers (STET); the registration jwks must contain the QSEALC\n    public key (\"kty\" RSA, \"\
  alg\" RS256, \"use\" sig).\n  sources:\n  - openapi/groupe-bpce-psd2-payments-openapi.yml\n  - https://apistore.groupebpce.com/api/psd2-registration\n- name: registration-client-credentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://www.<codetab>.live.api.89C3.com/stet/psd2/oauth/token\n  description: 'Registration API: generic client_id “PSD2_TPPRegister”, grant_type client_credentials, scope manageRegistration;\n    returns a temporary access token; POST /register returns the client_id used in all PSD2 methods.'\n  sources:\n  - https://apistore.groupebpce.com/api/psd2-registration\ndocs: https://apistore.groupebpce.com/api/psd2-registration\nclient_id_rule: client_id must equal the organization identifier from the eIDAS certificate distinguished name (ETSI\n  TS 119 495 §5.2.1), e.g. PSDFR-ACPR-12345.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/groupe-bpce/refs/heads/main/authentication/groupe-bpce-authentication.yml
summary_line: mutualTLS/oauth2 · 5 schemes
tags:
- Company
- Banking
- Financial Services
- Open Banking
- PSD2
- Payments
- Insurance
- France
---
