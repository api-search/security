---
api_key_in: []
api_specs:
- filename: acma-access-areas-api-openapi.yml
  format: yaml
  label: ACMA Access areas API
  slug: acma-access-areas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acma/refs/heads/main/openapi/acma-access-areas-api-openapi.yml
- filename: acma-antennas-api-openapi.yml
  format: yaml
  label: ACMA Antennas API
  slug: acma-antennas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acma/refs/heads/main/openapi/acma-antennas-api-openapi.yml
- filename: acma-clients-api-openapi.yml
  format: yaml
  label: ACMA Clients API
  slug: acma-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acma/refs/heads/main/openapi/acma-clients-api-openapi.yml
- filename: acma-licence-categories-api-openapi.yml
  format: yaml
  label: ACMA Licence categories API
  slug: acma-licence-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acma/refs/heads/main/openapi/acma-licence-categories-api-openapi.yml
- filename: acma-licences-api-openapi.yml
  format: yaml
  label: ACMA Licences API
  slug: acma-licences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acma/refs/heads/main/openapi/acma-licences-api-openapi.yml
- filename: acma-registrations-api-openapi.yml
  format: yaml
  label: ACMA Registrations API
  slug: acma-registrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acma/refs/heads/main/openapi/acma-registrations-api-openapi.yml
- filename: acma-sites-api-openapi.yml
  format: yaml
  label: ACMA Sites API
  slug: acma-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acma/refs/heads/main/openapi/acma-sites-api-openapi.yml
auth_types:
- none
- soap-body-credentials
- ssh-key
- session
description: ''
kind: authentication
layout: security
method: searched
name: Acma Authentication
name_suffix: Authentication
oauth_flows: []
overview: ACMA secures its APIs with none, soap-body-credentials, ssh-key, and session across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: ACMA
provider_slug: acma
scheme_count: 5
schemes:
- api: acma:spectrum-licensing
  description: 'The ACMA Spectrum Licensing API requires no authentication at all — no API key, no account, no registration, no Authorization header. Every one of the 22 REST operations and the SOAP endpoint answers anonymous requests. Verified live on 2026-07-25 against api.acma.gov.au/SpectrumLicensingAPIOuterService/OuterService.svc: all documented operations returned HTTP 200 with data on an anonymous request. Access is instead governed contractually, by the "Licence to use the Register of Radiocommunications Licences" terms, and technically by a 2,000-record cap per query.'
  evidence:
    verified_live: https://api.acma.gov.au/SpectrumLicensingAPIOuterService/OuterService.svc/CategoryListJSON
    verified_on: '2026-07-25'
    verified_status: 200
  name: none
  sources:
  - openapi/acma-spectrum-licensing-openapi.yml
  - wsdl/acma-spectrum-licensing.wsdl
  type: none
- api: acma:do-not-call-register-washing
  description: The Do Not Call Register Real Time Access washing service authenticates with an account identifier and passphrase passed as SOAP method parameters, not as HTTP credentials. Every published operation takes TelemarketerId (the Account ID) and TelemarketerPassword; WashOnlyUserId is supplied only when the wash is performed under a wash-only sub-account of the main administration account. Multi-factor authentication is NOT required on the real-time channel, but the passphrase used must match the passphrase set when MFA was configured on the account. Access additionally requires a paid washing subscription of type D or above.
  name: dncr-rta-account-credentials
  parameters:
  - description: The Account ID issued to the industry account holder.
    name: TelemarketerId
    required: true
  - description: The account passphrase; must match the passphrase used when setting up MFA on the account.
    name: TelemarketerPassword
    required: true
  - description: Supplied only when washing under a wash-only sub-account of the main account.
    name: WashOnlyUserId
    required: false
  sources:
  - wsdl/acma-dncr-realtime-washing.wsdl
  - https://www.donotcall.gov.au/getmedia/9810ca84-d7af-4972-b626-6b5495f52ac2/DNCR-SOAP-Fact-Sheet.pdf
  transport:
    note: ACMA states users are required to have TLS 1.2 to connect, and that client applications must be configured to force TLS 1.2 or above.
    tls_minimum: TLSv1.2
  type: soap-body-credentials
- api: acma:do-not-call-register-washing
  description: The Automated Washing Service batch channel authenticates over SFTP at sftp.donotcall.gov.au. Access seekers first connect with a username and a password issued by SMS to the registered mobile number, then upload an RSA public key (SSH-2 RSA, 2048-bit) into the account's /upload folder; subsequent connections use the key pair. Access is provisioned by emailing DNCR support with the organisation name, contact, mailing address, email, mobile number and the external public IP address of the device that will connect — the service is IP-restricted.
  directories:
  - upload
  - download
  - archive
  host: sftp.donotcall.gov.au
  name: dncr-sftp-ssh-key
  sources:
  - https://www.donotcall.gov.au/industry/washing-process-overview/sftp
  - https://www.donotcall.gov.au/getmedia/9b201a6a-6426-414a-a48d-0fdee2608ae1/dncr-ssh-key-authentication.pdf
  type: ssh-key
- api: null
  description: The ACMA developer portal at developer.acma.gov.au is a Microsoft Azure API Management developer portal behind a complete sign-in wall. Every anonymous request — /apis, /products, /api-docs — returns the identical sign-in shell, and the portal management API /mapi/apis returns HTTP 401. No API, product or specification is visible without an account. The /.well-known/openid-configuration and /.well-known/oauth-authorization-server paths return HTTP 200 but serve text/html (the SPA catch-all), not OIDC or RFC 8414 metadata, so no discoverable authorization server exists.
  evidence:
    content_type: text/html
    probed: https://developer.acma.gov.au/.well-known/openid-configuration
    status: 200
    verdict: SPA sign-in shell, not OIDC metadata
    verified_on: '2026-07-25'
  name: azure-apim-portal-signin
  sources:
  - well-known/acma-well-known.yml
  type: session
- api: null
  description: The ACMA Numbering System at thenumberingsystem.com.au is an authenticated web application for licensed carriage service providers. Its internal JSON backend under /app/* returns HTTP 401 to anonymous callers and is not offered or documented as an API.
  name: numbering-system-session
  sources:
  - review.yml
  type: session
slug: acma-authentication
source_filename: acma-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: >-\n  https://www.acma.gov.au/sites/default/files/2019-11/Spectrum%20licensing%20API.docx\ndocs:\n- https://www.acma.gov.au/sites/default/files/2019-11/Spectrum%20licensing%20API.docx\n- https://www.donotcall.gov.au/getmedia/9810ca84-d7af-4972-b626-6b5495f52ac2/DNCR-SOAP-Fact-Sheet.pdf\n- https://www.donotcall.gov.au/industry/washing-process-overview/sftp\nsummary:\n  types:\n  - none\n  - soap-body-credentials\n  - ssh-key\n  - session\n  api_key_in: []\n  oauth2_flows: []\n  note: >-\n    ACMA publishes no OAuth 2.0, OpenID Connect or API-key scheme on any public surface.\n    Its open register API is genuinely unauthenticated; its gated services carry credentials\n    in the SOAP body or over SSH rather than in HTTP auth headers.\nschemes:\n- name: none\n  api: acma:spectrum-licensing\n  type: none\n  description: >-\n    The ACMA Spectrum Licensing API requires no authentication at all — no API key, no\n    account, no\
  \ registration, no Authorization header. Every one of the 22 REST operations\n    and the SOAP endpoint answers anonymous requests. Verified live on 2026-07-25 against\n    api.acma.gov.au/SpectrumLicensingAPIOuterService/OuterService.svc: all documented\n    operations returned HTTP 200 with data on an anonymous request. Access is instead\n    governed contractually, by the \"Licence to use the Register of Radiocommunications\n    Licences\" terms, and technically by a 2,000-record cap per query.\n  sources:\n  - openapi/acma-spectrum-licensing-openapi.yml\n  - wsdl/acma-spectrum-licensing.wsdl\n  evidence:\n    verified_live: https://api.acma.gov.au/SpectrumLicensingAPIOuterService/OuterService.svc/CategoryListJSON\n    verified_status: 200\n    verified_on: '2026-07-25'\n- name: dncr-rta-account-credentials\n  api: acma:do-not-call-register-washing\n  type: soap-body-credentials\n  description: >-\n    The Do Not Call Register Real Time Access washing service authenticates with an\n\
  \    account identifier and passphrase passed as SOAP method parameters, not as HTTP\n    credentials. Every published operation takes TelemarketerId (the Account ID) and\n    TelemarketerPassword; WashOnlyUserId is supplied only when the wash is performed\n    under a wash-only sub-account of the main administration account. Multi-factor\n    authentication is NOT required on the real-time channel, but the passphrase used\n    must match the passphrase set when MFA was configured on the account. Access\n    additionally requires a paid washing subscription of type D or above.\n  parameters:\n  - name: TelemarketerId\n    required: true\n    description: The Account ID issued to the industry account holder.\n  - name: TelemarketerPassword\n    required: true\n    description: The account passphrase; must match the passphrase used when setting up MFA on the account.\n  - name: WashOnlyUserId\n    required: false\n    description: Supplied only when washing under a wash-only sub-account\
  \ of the main account.\n  transport:\n    tls_minimum: TLSv1.2\n    note: >-\n      ACMA states users are required to have TLS 1.2 to connect, and that client applications\n      must be configured to force TLS 1.2 or above.\n  sources:\n  - wsdl/acma-dncr-realtime-washing.wsdl\n  - https://www.donotcall.gov.au/getmedia/9810ca84-d7af-4972-b626-6b5495f52ac2/DNCR-SOAP-Fact-Sheet.pdf\n- name: dncr-sftp-ssh-key\n  api: acma:do-not-call-register-washing\n  type: ssh-key\n  description: >-\n    The Automated Washing Service batch channel authenticates over SFTP at\n    sftp.donotcall.gov.au. Access seekers first connect with a username and a password\n    issued by SMS to the registered mobile number, then upload an RSA public key (SSH-2\n    RSA, 2048-bit) into the account's /upload folder; subsequent connections use the key\n    pair. Access is provisioned by emailing DNCR support with the organisation name,\n    contact, mailing address, email, mobile number and the external public IP address\
  \ of\n    the device that will connect — the service is IP-restricted.\n  host: sftp.donotcall.gov.au\n  directories:\n  - upload\n  - download\n  - archive\n  sources:\n  - https://www.donotcall.gov.au/industry/washing-process-overview/sftp\n  - https://www.donotcall.gov.au/getmedia/9b201a6a-6426-414a-a48d-0fdee2608ae1/dncr-ssh-key-authentication.pdf\n- name: azure-apim-portal-signin\n  api: null\n  type: session\n  description: >-\n    The ACMA developer portal at developer.acma.gov.au is a Microsoft Azure API Management\n    developer portal behind a complete sign-in wall. Every anonymous request — /apis,\n    /products, /api-docs — returns the identical sign-in shell, and the portal management\n    API /mapi/apis returns HTTP 401. No API, product or specification is visible without\n    an account. The /.well-known/openid-configuration and /.well-known/oauth-authorization-server\n    paths return HTTP 200 but serve text/html (the SPA catch-all), not OIDC or RFC 8414\n    metadata,\
  \ so no discoverable authorization server exists.\n  sources:\n  - well-known/acma-well-known.yml\n  evidence:\n    probed: https://developer.acma.gov.au/.well-known/openid-configuration\n    status: 200\n    content_type: text/html\n    verdict: SPA sign-in shell, not OIDC metadata\n    verified_on: '2026-07-25'\n- name: numbering-system-session\n  api: null\n  type: session\n  description: >-\n    The ACMA Numbering System at thenumberingsystem.com.au is an authenticated web\n    application for licensed carriage service providers. Its internal JSON backend under\n    /app/* returns HTTP 401 to anonymous callers and is not offered or documented as an API.\n  sources:\n  - review.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acma/refs/heads/main/authentication/acma-authentication.yml
summary_line: none/soap-body-credentials/ssh-key/session · 5 schemes
tags:
- Telecommunications
- Australia
- Regulator
- Spectrum
- Broadcasting
- Numbering
- Do Not Call Register
- Radiocommunications
- Licensing
- Open Data
- Government
- SOAP
---
