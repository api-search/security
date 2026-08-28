---
api_key_in: []
api_specs:
- filename: simba-chain-member-service-openapi.json
  format: json
  label: SIMBA Blocks Member Service API
  slug: simba-chain-member-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simba-chain/refs/heads/main/openapi/simba-chain-member-service-openapi.json
- filename: simba-chain-member-service-validator-openapi.json
  format: json
  label: SIMBA Blocks Authentication Service API
  slug: simba-chain-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simba-chain/refs/heads/main/openapi/simba-chain-member-service-validator-openapi.json
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Simba Chain Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- refreshToken
overview: SIMBA Chain secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, and refreshToken flow(s).
provider_name: SIMBA Chain
provider_slug: simba-chain
scheme_count: 2
schemes:
- flows:
  - authorizationUrl: https://blocks.simbachain.com/api/member-service-validator/oauth/authorize
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://blocks.simbachain.com/api/member-service-validator/oauth/token
  name: OAuth2AuthorizationCodeBearer
  sources:
  - openapi/simba-chain-member-service-openapi.json
  type: oauth2
- declared_in_spec: false
  evidence: Not declared as a securityScheme, but it is the flow every SIMBA SDK and CLI actually uses. grant_types_supported in the OIDC discovery document includes client_credentials; the authentication OpenAPI defines a ClientCredentialParams request schema (grant_type, client_id, client_secret); and the Python SDK docs state "The AUTH_FLOW should currently not be changed as only client_credentials is supported."
  flow: clientCredentials
  name: client_credentials
  sources:
  - well-known/simba-chain-openid-configuration.json
  - openapi/simba-chain-member-service-validator-openapi.json
  - https://docs.simbachain.com/documentation/developer-resources/simba-sdks/python-sdk
  tokenUrl: https://blocks.simbachain.com/api/member-service-validator/oauth/token
  type: oauth2
slug: simba-chain-authentication
source_filename: simba-chain-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: searched\nsource: >-\n  Baseline derived by 0-working/derive-authentication.py from\n  openapi/simba-chain-member-service-openapi.json, then upgraded from\n  https://docs.simbachain.com/documentation/getting-started/obtaining-api-keys,\n  /developer-resources/environmental-variables, /developer-resources/simba-sdks/python-sdk,\n  /getting-started/quickstart-guides/api-quickstart, and the provider's live OIDC discovery document\n  (HTTP 200, fetched 2026-08-27, saved to well-known/simba-chain-openid-configuration.json).\ndocs: https://docs.simbachain.com/documentation/getting-started/obtaining-api-keys\nsummary:\n  types:\n    - oauth2\n    - openIdConnect\n  oauth2_flows:\n    - authorizationCode\n    - clientCredentials\n    - refreshToken\n  api_keys: false\n  http_basic: false\n  mutual_tls: false\nschemes:\n  - name: OAuth2AuthorizationCodeBearer\n    type: oauth2\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://blocks.simbachain.com/api/member-service-validator/oauth/authorize\n\
  \        tokenUrl: https://blocks.simbachain.com/api/member-service-validator/oauth/token\n        scopes: 0\n    sources:\n      - openapi/simba-chain-member-service-openapi.json\n  - name: client_credentials\n    type: oauth2\n    flow: clientCredentials\n    tokenUrl: https://blocks.simbachain.com/api/member-service-validator/oauth/token\n    declared_in_spec: false\n    evidence: >-\n      Not declared as a securityScheme, but it is the flow every SIMBA SDK and CLI actually uses.\n      grant_types_supported in the OIDC discovery document includes client_credentials; the\n      authentication OpenAPI defines a ClientCredentialParams request schema\n      (grant_type, client_id, client_secret); and the Python SDK docs state \"The AUTH_FLOW should\n      currently not be changed as only client_credentials is supported.\"\n    sources:\n      - well-known/simba-chain-openid-configuration.json\n      - openapi/simba-chain-member-service-validator-openapi.json\n      - https://docs.simbachain.com/documentation/developer-resources/simba-sdks/python-sdk\n\
  openid_connect:\n  discovery: https://blocks.simbachain.com/api/member-service-validator/oauth/.well-known/openid-configuration\n  discovery_saved: well-known/simba-chain-openid-configuration.json\n  jwks_uri: https://blocks.simbachain.com/api/member-service-validator/oauth/.well-known/jwks\n  jwks_saved: well-known/simba-chain-jwks.json\n  issuer: simba://authservice\n  issuer_deviation: >-\n    The issuer is a simba:// URI, not an https URL. That is off-spec for OpenID Connect Discovery and\n    will fail strict relying-party issuer validation.\n  userinfo_endpoint: https://blocks.simbachain.com/api/member-service-validator/oauth/userinfo\n  end_session_endpoint: https://blocks.simbachain.com/api/member-service-validator/oauth/logout\n  response_types_supported: [code]\n  id_token_signing_alg_values_supported: [RS256]\n  token_endpoint_auth_methods_supported: [client_secret_post, client_secret_basic, none]\n  code_challenge_methods_supported: [S256]\n  scopes_supported: [openid, email,\
  \ profile]\n  signing_keys: 1 RSA key (RS256), kid 2ecb858a-8f72-40b5-846c-a3f21eab4e43\ncredentials:\n  name: Secret Key Pair (client ID + client secret)\n  where_to_get: >-\n    SIMBA Build UI: organisation -> application -> Secrets, or user Profile -> Secrets -> New Secret.\n    Programmatically via the Member Service ClientCredentials operations.\n  one_time_display: >-\n    \"This will be the only time the secret value is shown, so be sure to save it somewhere safe.\"\n  rotation: refresh_client_credential_secret_organisations__organisation_name__client_credentials__client_id__refresh_put\n  revocation: revoke_client_credential_organisations__organisation_name__client_credentials__client_id__delete\n  expiry_field: expire_at\n  last_used_field: last_used\n  scoping: A credential is scoped to a user or an organisation, and carries its own role assignments.\n  impersonation: >-\n    create_impersonate_user_client_credentials_user_accounts__user_account_id__client_credentials__post\n\
  \    mints a credential that acts as a given user (impersonate_user field on ClientCredential).\nconfiguration:\n  env_vars:\n    SIMBA_API_BASE_URL: The Blocks instance base URL, e.g. https://blocks.simbachain.com or a customer's own instance.\n    SIMBA_AUTH_BASE_URL: Same as SIMBA_API_BASE_URL for the default Blocks auth provider; the Keycloak host when SIMBA_AUTH_PROVIDER=KC.\n    SIMBA_AUTH_CLIENT_ID: The API Secret Key.\n    SIMBA_AUTH_CLIENT_SECRET: The API Client Secret.\n    SIMBA_AUTH_PROVIDER: Blocks (default) or KC for Keycloak.\n    SIMBA_AUTH_REALM: Keycloak realm, e.g. simbachain (Keycloak only).\n    SIMBA_HOME: Directory holding the dotenv file when it is not in the project root.\n  dotenv_names: ['.simbachain.env', 'simbachain.env', '.env']\n  docs: https://docs.simbachain.com/documentation/developer-resources/environmental-variables\n  alternative_providers:\n    - name: Blocks (built-in)\n      note: SIMBA_AUTH_BASE_URL == SIMBA_API_BASE_URL.\n    - name: Keycloak\n\
  \      note: SIMBA_AUTH_PROVIDER=KC with SIMBA_AUTH_REALM; SIMBA_AUTH_BASE_URL points at the Keycloak server.\nadditional_factors:\n  totp:\n    supported: true\n    operations: [get_setup_account_security_2fa_setup_get, post_setup_verify_account_security_2fa_setup_verify_post, post_setup_acknowledge_account_security_2fa_setup_acknowledge_post, post_disable_account_security_2fa_disable_post, get_recovery_codes_show_account_security_2fa_recovery_codes_show_get, post_recovery_codes_regenerate_account_security_2fa_recovery_codes_regenerate_post]\n  passkeys:\n    supported: true\n    standard: WebAuthn / FIDO2\n    operations: [list_passkeys_account_security_passkeys_get, post_register_options_account_security_passkeys_register_options_post, post_register_verify_account_security_passkeys_register_verify_post, post_rename_passkey_account_security_passkeys__credential_pk__rename_post, post_delete_passkey_account_security_passkeys__credential_pk__delete_post]\n  verifiable_presentation:\n  \
  \  supported: true\n    operation: get_vc_secure_session_oauth_vc_secure_session_post\n    request: 'GetVcSecureParams { registrant_did_id }'\n    response: VPChallenge\n    optional_header: dpop (RFC 9449 proof of possession)\n    note: Binds a W3C DID-held Verifiable Credential to a session; see conformance/simba-chain-conformance.yml.\ndelegation:\n  header: txn-delegate\n  description: >-\n    On the dynamic contract API, identifies an external user on whose behalf a transaction is signed.\n    Requires delegation permission for the organisation. The delegated identifier is opaque to Blocks.\n  docs: https://docs.simbachain.com/documentation/getting-started/quickstart-guides/api-quickstart\nobserved:\n  - url: https://blocks.simbachain.com/api/member-service/pingz\n    status: 401\n    body: '{\"detail\":\"missing-auth-header\"}'\n    note: Anonymous probe 2026-08-27 — the missing-credential response shape.\n  - url: https://blocks.simbachain.com/api/platform-service/v2/\n    status:\
  \ 401\n    body: '{\"detail\":\"missing-auth-header\"}'\n    note: Anonymous probe 2026-08-27 — the dynamic contract API is gated at the gateway.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/simba-chain/refs/heads/main/authentication/simba-chain-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- Blockchain
- Supply Chain
- Traceability
- Digital Product Passport
- Smart Contracts
- Identity
- Verifiable Credentials
- Defense
- Government
- Data Management
---
