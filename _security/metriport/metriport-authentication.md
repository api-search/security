---
api_key_in:
- header
api_specs:
- filename: metriport-consolidated-api-openapi.yml
  format: yaml
  label: Metriport Consolidated API
  slug: metriport-consolidated-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metriport/refs/heads/main/openapi/metriport-consolidated-api-openapi.yml
- filename: metriport-devices-data-api-openapi.yml
  format: yaml
  label: Metriport Devices Data API
  slug: metriport-devices-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metriport/refs/heads/main/openapi/metriport-devices-data-api-openapi.yml
- filename: metriport-document-api-openapi.yml
  format: yaml
  label: Metriport Document API
  slug: metriport-document-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metriport/refs/heads/main/openapi/metriport-document-api-openapi.yml
- filename: metriport-facility-api-openapi.yml
  format: yaml
  label: Metriport Facility API
  slug: metriport-facility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metriport/refs/heads/main/openapi/metriport-facility-api-openapi.yml
- filename: metriport-patient-api-openapi.yml
  format: yaml
  label: Metriport Patient API
  slug: metriport-patient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metriport/refs/heads/main/openapi/metriport-patient-api-openapi.yml
- filename: metriport-settings-api-openapi.yml
  format: yaml
  label: Metriport Settings API
  slug: metriport-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metriport/refs/heads/main/openapi/metriport-settings-api-openapi.yml
- filename: metriport-user-api-openapi.yml
  format: yaml
  label: Metriport User API
  slug: metriport-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metriport/refs/heads/main/openapi/metriport-user-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Metriport Authentication
name_suffix: Authentication
oauth_flows: []
overview: Metriport secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Metriport
provider_slug: metriport
scheme_count: 1
schemes:
- detail: A single static key grants full access to the account, including destructive operations. There are no scopes, no restricted or read-only keys, and no per-facility scoping. Metriport's own guidance is to treat the key like an account password and use it only from backend services.
  environments:
  - base_url: https://api.metriport.com
    name: production
  - base_url: https://api.sandbox.metriport.com
    name: sandbox
    note: Minted separately after toggling Sandbox mode in the dashboard; not interchangeable with production keys.
  in: header
  key_format:
    note: Metriport publishes no distinguishing key prefix for sandbox versus production. A client cannot tell which environment a key belongs to by inspecting it, and a leaked key has no scannable shape.
    prefix: none published
  key_management:
    issued_from: https://dash.metriport.com/developers
    max_active_keys: 2
    revocation: Immediate — revoking a key on the Developers page makes it inactive at once.
    rotation: Both keys are equally privileged and interchangeable, so rotation is generate-new, roll-out, revoke-old with zero downtime.
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/metriport-consolidated-api-openapi.yml
  - openapi/metriport-devices-data-api-openapi.yml
  - openapi/metriport-document-api-openapi.yml
  - openapi/metriport-facility-api-openapi.yml
  - openapi/metriport-patient-api-openapi.yml
  - openapi/metriport-settings-api-openapi.yml
  - openapi/metriport-user-api-openapi.yml
  - https://docs.metriport.com/medical-api/getting-started/api-keys
  type: apiKey
slug: metriport-authentication
source_filename: metriport-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\ndocs: https://docs.metriport.com/medical-api/getting-started/api-keys\nsource: >-\n  https://docs.metriport.com/medical-api/getting-started/api-keys,\n  /medical-api/more-info/sso, /medical-api/getting-started/embedding,\n  /medical-api/getting-started/webhooks; scheme confirmed against the\n  securitySchemes in openapi/*.yml.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/metriport-consolidated-api-openapi.yml\n  - openapi/metriport-devices-data-api-openapi.yml\n  - openapi/metriport-document-api-openapi.yml\n  - openapi/metriport-facility-api-openapi.yml\n  - openapi/metriport-patient-api-openapi.yml\n  - openapi/metriport-settings-api-openapi.yml\n  - openapi/metriport-user-api-openapi.yml\n  - https://docs.metriport.com/medical-api/getting-started/api-keys\n  detail: >-\n    A single static key grants full access\
  \ to the account, including destructive\n    operations. There are no scopes, no restricted or read-only keys, and no\n    per-facility scoping. Metriport's own guidance is to treat the key like an\n    account password and use it only from backend services.\n  key_management:\n    issued_from: https://dash.metriport.com/developers\n    max_active_keys: 2\n    rotation: >-\n      Both keys are equally privileged and interchangeable, so rotation is\n      generate-new, roll-out, revoke-old with zero downtime.\n    revocation: Immediate — revoking a key on the Developers page makes it inactive at once.\n  environments:\n  - name: production\n    base_url: https://api.metriport.com\n  - name: sandbox\n    base_url: https://api.sandbox.metriport.com\n    note: Minted separately after toggling Sandbox mode in the dashboard; not interchangeable with production keys.\n  key_format:\n    prefix: none published\n    note: >-\n      Metriport publishes no distinguishing key prefix for sandbox versus\n\
  \      production. A client cannot tell which environment a key belongs to by\n      inspecting it, and a leaked key has no scannable shape.\noauth2: false\noidc: false\nmtls: false\nadjacent_credentials:\n- name: Embed token\n  type: URL-borne bearer token\n  parameter: access_token (query parameter on the embedded app URL)\n  minted_by: POST /medical/v1/token/embed, server-side, using the API key\n  max_lifetime_seconds: 36000\n  purpose: Authorises the hosted embedded app (Patient View, Transitions of Care) in a browser.\n  docs: https://docs.metriport.com/medical-api/getting-started/embedding\n- name: Webhook key\n  type: HMAC shared secret\n  parameter: x-metriport-signature (on inbound requests FROM Metriport)\n  algorithm: HMAC-SHA256 over the raw body\n  purpose: Lets your endpoint verify that a webhook came from Metriport.\n  rotation: Clear and re-set the webhook URL to regenerate.\n  docs: https://docs.metriport.com/medical-api/getting-started/webhooks\n- name: SAML / Enterprise\
  \ SSO\n  type: SAML 2.0\n  purpose: >-\n    Human sign-in to the Metriport dashboard only — NOT an API authentication\n    method. Named IdP guides for Google, Okta, Azure, OneLogin, JumpCloud, Duo\n    and Rippling; attribute mapping on email, first_name, last_name.\n  docs: https://docs.metriport.com/medical-api/more-info/sso\ngaps:\n- No OAuth 2.0 or OIDC; no delegated or third-party authorisation flow.\n- No scoped, restricted or read-only API keys — least privilege is not expressible.\n- No mutual TLS.\n- No key-prefix convention, so leaked keys cannot be pattern-detected by secret scanners.\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/metriport/refs/heads/main/authentication/metriport-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Healthcare
- Medical Records
- FHIR
- Health Data
- Wearables
- Open-Source
---
