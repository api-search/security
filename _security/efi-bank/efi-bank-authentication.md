---
api_key_in: []
api_specs:
- filename: efi-bank-openapi.yml
  format: yaml
  label: Efí Pix Charges API
  slug: efi-bank-pix-charges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/efi-bank/refs/heads/main/openapi/efi-bank-openapi.yml
- filename: efi-bank-openapi.yml
  format: yaml
  label: Efí Pix Payments API
  slug: efi-bank-pix-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/efi-bank/refs/heads/main/openapi/efi-bank-openapi.yml
- filename: efi-bank-openapi.yml
  format: yaml
  label: Efí Pix Webhooks API
  slug: efi-bank-pix-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/efi-bank/refs/heads/main/openapi/efi-bank-openapi.yml
- filename: efi-bank-openapi.yml
  format: yaml
  label: Efí Cobranças (Charges) API
  slug: efi-bank-cobrancas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/efi-bank/refs/heads/main/openapi/efi-bank-openapi.yml
- filename: efi-bank-openapi.yml
  format: yaml
  label: Efí Carnê API
  slug: efi-bank-carne-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/efi-bank/refs/heads/main/openapi/efi-bank-openapi.yml
- filename: efi-bank-openapi.yml
  format: yaml
  label: Efí Pix via Open Finance API
  slug: efi-bank-open-finance-pix-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/efi-bank/refs/heads/main/openapi/efi-bank-openapi.yml
auth_types:
- oauth2
- mutualTLS
description: ''
kind: authentication
layout: security
method: derived
name: Efi Bank Authentication
name_suffix: Authentication
oauth_flows: []
overview: Efí secures its APIs with oauth2 and mutualTLS across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Efí
provider_slug: efi-bank
scheme_count: 2
schemes:
- description: 'OAuth2 client-credentials across all Efí hosts. Obtain a bearer token from the host''s token endpoint using HTTP Basic auth with Client_Id and Client_Secret, then send it as `Authorization: Bearer`. Token endpoints differ per host: Pix `POST /oauth/token` (https://pix.api.efipay.com.br), Cobranças `POST /v1/authorize` (https://cobrancas.api.efipay.com.br), Open Finance `POST /v1/oauth/token` (https://openfinance.api.efipay.com.br). Access is scoped (cob.write, cob.read, pix.read, pix.send, webhook.write, gn.opb.payment.pix.send, etc).'
  flow: clientCredentials
  name: oAuth2ClientCredentials
  sources:
  - openapi/efi-bank-openapi.yml
  - https://dev.efipay.com.br/docs/api-pix/credenciais
  - https://dev.efipay.com.br/docs/api-cobrancas/credenciais
  type: oauth2
- description: Mutual TLS (mTLS) client certificate is MANDATORY on every request to the Pix and Open Finance hosts, including the OAuth2 token request. Efí issues a `.p12` (PKCS#12) certificate in the account dashboard, which can be converted to `.pem`. This is a Brazilian Central Bank (BACEN) requirement for the Pix arrangement, not an Efí-specific choice. The Cobranças (Charges / Carnê) host does NOT require mTLS - OAuth2 alone is sufficient there. mTLS cannot be fully expressed as an OpenAPI 3.0 security scheme, so it is documented separately here and in prose within the OpenAPI description.
  name: mutualTLS
  notRequiredOnHosts:
  - https://cobrancas.api.efipay.com.br
  requiredOnHosts:
  - https://pix.api.efipay.com.br
  - https://openfinance.api.efipay.com.br
  sources:
  - https://dev.efipay.com.br/docs/api-pix/credenciais
  - https://dev.efipay.com.br/docs/api-open-finance/credenciais
  type: mutualTLS
slug: efi-bank-authentication
source_filename: efi-bank-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: derived\nsource: openapi/efi-bank-openapi.yml\nsummary:\n  types:\n  - oauth2\n  - mutualTLS\nschemes:\n- name: oAuth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  description: >-\n    OAuth2 client-credentials across all Efí hosts. Obtain a bearer token from\n    the host's token endpoint using HTTP Basic auth with Client_Id and\n    Client_Secret, then send it as `Authorization: Bearer`. Token endpoints\n    differ per host: Pix `POST /oauth/token`\n    (https://pix.api.efipay.com.br), Cobranças `POST /v1/authorize`\n    (https://cobrancas.api.efipay.com.br), Open Finance `POST /v1/oauth/token`\n    (https://openfinance.api.efipay.com.br). Access is scoped (cob.write,\n    cob.read, pix.read, pix.send, webhook.write, gn.opb.payment.pix.send, etc).\n  sources:\n  - openapi/efi-bank-openapi.yml\n  - https://dev.efipay.com.br/docs/api-pix/credenciais\n  - https://dev.efipay.com.br/docs/api-cobrancas/credenciais\n- name: mutualTLS\n\
  \  type: mutualTLS\n  description: >-\n    Mutual TLS (mTLS) client certificate is MANDATORY on every request to the\n    Pix and Open Finance hosts, including the OAuth2 token request. Efí issues a\n    `.p12` (PKCS#12) certificate in the account dashboard, which can be converted\n    to `.pem`. This is a Brazilian Central Bank (BACEN) requirement for the Pix\n    arrangement, not an Efí-specific choice. The Cobranças (Charges / Carnê) host\n    does NOT require mTLS - OAuth2 alone is sufficient there. mTLS cannot be fully\n    expressed as an OpenAPI 3.0 security scheme, so it is documented separately\n    here and in prose within the OpenAPI description.\n  requiredOnHosts:\n  - https://pix.api.efipay.com.br\n  - https://openfinance.api.efipay.com.br\n  notRequiredOnHosts:\n  - https://cobrancas.api.efipay.com.br\n  sources:\n  - https://dev.efipay.com.br/docs/api-pix/credenciais\n  - https://dev.efipay.com.br/docs/api-open-finance/credenciais\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/efi-bank/refs/heads/main/authentication/efi-bank-authentication.yml
summary_line: oauth2/mutualTLS · 2 schemes
tags:
- Payments
- Pix
- Boleto
- Banking
- Brazil
- Latin America
- Charges
- Digital Account
- Financial Infrastructure
- Fintech
---
