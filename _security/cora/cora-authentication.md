---
api_key_in: []
auth_types:
- oauth2
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Cora Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Cora secures its APIs with oauth2 and mutualTLS across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Cora
provider_slug: cora
scheme_count: 2
schemes:
- description: Client certificate (certificate.pem) + private key (private-key.key) presented on every request for the Direct Integration modality (matls-clients hosts).
  modality: direct-integration
  name: mutualTLS
  sources:
  - docs:developers.cora.com.br/docs/client-credentials-int-direta
  type: mutualTLS
- description: POST grant_type=client_credentials&client_id=<client_id> to /token (presenting the client certificate + key for Direct Integration) to receive a Bearer access token used in the Authorization header of subsequent API calls.
  flow: clientCredentials
  grant_type: client_credentials
  name: OAuth2ClientCredentials
  parameters:
  - client_id
  request_content_type: application/x-www-form-urlencoded
  sources:
  - docs:developers.cora.com.br/docs/client-credentials-int-direta
  token_type: Bearer
  token_url_production: https://matls-clients.api.cora.com.br/token
  token_url_stage: https://matls-clients.api.stage.cora.com.br/token
  type: oauth2
slug: cora-authentication
source_filename: cora-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://developers.cora.com.br/docs/client-credentials-int-direta\ndocs: https://developers.cora.com.br/docs/client-credentials-int-direta\nsummary:\n  types:\n  - oauth2\n  - mutualTLS\n  oauth2_flows:\n  - clientCredentials\n  notes: >-\n    Cora offers two integration modalities. Direct Integration (Integração Direta)\n    requires mutual TLS: every request must present an X.509 client certificate and\n    private key issued by Cora, in addition to an OAuth2 client-credentials bearer\n    token obtained from the /token endpoint. Cora Partnership (Parceria Cora) uses\n    OAuth2 client-credentials with a client secret (no client certificate). Credentials\n    are provisioned through the Cora app or Cora Web, not self-service.\nschemes:\n- name: mutualTLS\n  type: mutualTLS\n  description: >-\n    Client certificate (certificate.pem) + private key (private-key.key) presented\n    on every request for the Direct Integration\
  \ modality (matls-clients hosts).\n  modality: direct-integration\n  sources:\n  - docs:developers.cora.com.br/docs/client-credentials-int-direta\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  token_url_stage: https://matls-clients.api.stage.cora.com.br/token\n  token_url_production: https://matls-clients.api.cora.com.br/token\n  grant_type: client_credentials\n  token_type: Bearer\n  request_content_type: application/x-www-form-urlencoded\n  parameters:\n  - client_id\n  description: >-\n    POST grant_type=client_credentials&client_id=<client_id> to /token (presenting\n    the client certificate + key for Direct Integration) to receive a Bearer access\n    token used in the Authorization header of subsequent API calls.\n  sources:\n  - docs:developers.cora.com.br/docs/client-credentials-int-direta\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cora/refs/heads/main/authentication/cora-authentication.yml
summary_line: oauth2/mutualTLS · 2 schemes
tags:
- Company
- Banking
- Brazil
- Payments
- Pix
- Boleto
- Invoicing
- SMB
- Fintech
- Banking-as-a-Service
---
