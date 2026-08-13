---
api_key_in: []
auth_types: []
description: 'Empatica publishes no OpenAPI and no public API reference, so this profile is assembled from the provider''s own support documentation for Data Access Keys and from anonymous probes of the live api.empatica.com host. There is no OAuth 2.0 or OpenID Connect surface anywhere: /.well-known/openid-configuration and /.well-known/oauth-authorization-server 404 on api.empatica.com and are soft-404 HTML shells on www and care. Consequently no scopes/ artifact is emitted — there is no scope surface to describe.'
kind: authentication
layout: security
method: searched
name: Empatica Authentication
name_suffix: Authentication
oauth_flows: []
overview: Empatica declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Empatica
provider_slug: empatica
scheme_count: 3
schemes:
- applies_to: empatica-cloud-data-access
  credentials:
  - description: AWS Access Key ID used to connect to the Empatica S3 bucket.
    name: ACCESS KEY ID
  - description: AWS Secret Access Key. Shown once, at generation time, and downloadable as CSV. Not retrievable afterwards.
    name: SECRET ACCESS KEY
  - description: Organization-specific data location, of the form s3://bucket-name/version/dir-name/.
    name: S3 ACCESS URL
  description: AWS Access Key ID + Secret Access Key pair, issued by Empatica and scoped to the organization's S3 prefix. Presented as ordinary AWS Signature Version 4 credentials by whatever S3 client is used (Cyberduck, AWS CLI v2, an AWS SDK).
  documented: true
  id: data-access-keys
  in: header
  issuance:
    delivery: Displayed in the portal once; downloadable as CSV.
    max_active_key_sets: 2
    revocation: Irreversible. Revoking invalidates all previously validated tokens and breaks every application using that key set. One slot re-opens for a new set.
    rotation: A new key set can only be generated once an existing set is revoked, so rotation is a revoke-then-generate operation rather than an overlap.
    self_service: true
    surface: Care Portal → Data → Data Access Keys
  method: searched
  provider_guidance:
  - Treat access keys as secret; never publish or expose them.
  - Never commit keys in plain text to a versioning system such as Git.
  - Use environment variables or a secrets-management tool.
  source: https://support.empatica.com/hc/en-us/articles/16650715124125-Generating-and-Revoking-Data-Access-Keys
  type: aws-sigv4
- applies_to: empatica-platform-api
  cors_advertised_headers:
  - origin
  - x-requested-with
  - content-type
  - accept
  - authorization
  - x-emp-app-version
  - x-emp-app-name
  - x-emp-app-platform
  - x-forwarded-for
  - elastic-apm-traceparent
  description: api.empatica.com/v2 is a token-protected REST host. A bearer token is exchanged at POST /v2/login; protected routes reject an anonymous or unrecognised token with HTTP 401 and errorCode 3998 "Missing token". Empatica publishes no reference for this host — every field below is probe evidence recorded on 2026-08-12, not documentation.
  documented: false
  grant: username/password exchanged for a token (form/JSON body; body schema not published)
  header: Authorization
  id: platform-bearer-token
  in: header
  method: probed
  scheme: bearer
  token_endpoint: https://api.empatica.com/v2/login
  type: http
  x-evidence:
  - body: '{}'
    http_status: 401
    method: POST
    response: '{"status":"error","statusText":"Unauthorized","errorCode":3010,"payload":"Invalid username or password"}'
    url: https://api.empatica.com/v2/login
  - auth: none
    http_status: 401
    method: GET
    response: '{"status":"Missing token","statusText":"","errorCode":3998}'
    url: https://api.empatica.com/v2/users/me
  - auth: Bearer <invalid>
    http_status: 401
    method: GET
    response: '{"status":"Missing token","statusText":"","errorCode":3998}'
    url: https://api.empatica.com/v2/users/me
  - auth: none
    http_status: 401
    method: POST
    response: '{"status":"Missing token","statusText":"","errorCode":3998}'
    url: https://api.empatica.com/v2/devices
- applies_to: empatica-cloud-api
  description: The Cloud API's authentication model is not published. Empatica states on https://www.empatica.com/cloud-api/ that "All Cloud API clients will be provided with full developer documentation", so the auth scheme is disclosed only after a contract is in place. Recorded as unknown rather than guessed.
  documented: false
  id: cloud-api-credentials
  method: none
  type: unknown
  x-evidence:
  - base URL or reference published: null
    finding: no auth scheme
    http_status: 200
    url: https://www.empatica.com/cloud-api/
slug: empatica-authentication
source_filename: empatica-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: https://support.empatica.com/hc/en-us/articles/16650715124125-Generating-and-Revoking-Data-Access-Keys\ndocs:\n- https://support.empatica.com/hc/en-us/articles/16650715124125-Generating-and-Revoking-Data-Access-Keys\n- https://support.empatica.com/hc/en-us/articles/13879014347421-Accessing-Data-on-the-S3-Bucket\nname: Empatica authentication profile\ndescription: >-\n  Empatica publishes no OpenAPI and no public API reference, so this profile is\n  assembled from the provider's own support documentation for Data Access Keys\n  and from anonymous probes of the live api.empatica.com host. There is no OAuth\n  2.0 or OpenID Connect surface anywhere: /.well-known/openid-configuration and\n  /.well-known/oauth-authorization-server 404 on api.empatica.com and are\n  soft-404 HTML shells on www and care. Consequently no scopes/ artifact is\n  emitted — there is no scope surface to describe.\nschemes:\n- id: data-access-keys\n  applies_to:\
  \ empatica-cloud-data-access\n  type: aws-sigv4\n  in: header\n  method: searched\n  documented: true\n  description: >-\n    AWS Access Key ID + Secret Access Key pair, issued by Empatica and scoped to\n    the organization's S3 prefix. Presented as ordinary AWS Signature Version 4\n    credentials by whatever S3 client is used (Cyberduck, AWS CLI v2, an AWS SDK).\n  credentials:\n  - name: ACCESS KEY ID\n    description: AWS Access Key ID used to connect to the Empatica S3 bucket.\n  - name: SECRET ACCESS KEY\n    description: AWS Secret Access Key. Shown once, at generation time, and downloadable\n      as CSV. Not retrievable afterwards.\n  - name: S3 ACCESS URL\n    description: 'Organization-specific data location, of the form s3://bucket-name/version/dir-name/.'\n  issuance:\n    surface: Care Portal → Data → Data Access Keys\n    self_service: true\n    max_active_key_sets: 2\n    rotation: >-\n      A new key set can only be generated once an existing set is revoked, so\n    \
  \  rotation is a revoke-then-generate operation rather than an overlap.\n    revocation: >-\n      Irreversible. Revoking invalidates all previously validated tokens and\n      breaks every application using that key set. One slot re-opens for a new set.\n    delivery: Displayed in the portal once; downloadable as CSV.\n  provider_guidance:\n  - Treat access keys as secret; never publish or expose them.\n  - Never commit keys in plain text to a versioning system such as Git.\n  - Use environment variables or a secrets-management tool.\n  source: https://support.empatica.com/hc/en-us/articles/16650715124125-Generating-and-Revoking-Data-Access-Keys\n- id: platform-bearer-token\n  applies_to: empatica-platform-api\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  method: probed\n  documented: false\n  description: >-\n    api.empatica.com/v2 is a token-protected REST host. A bearer token is\n    exchanged at POST /v2/login; protected routes reject an anonymous or\n\
  \    unrecognised token with HTTP 401 and errorCode 3998 \"Missing token\".\n    Empatica publishes no reference for this host — every field below is probe\n    evidence recorded on 2026-08-12, not documentation.\n  token_endpoint: https://api.empatica.com/v2/login\n  grant: username/password exchanged for a token (form/JSON body; body schema not\n    published)\n  x-evidence:\n  - {url: 'https://api.empatica.com/v2/login', method: POST, body: '{}', http_status: 401,\n    response: '{\"status\":\"error\",\"statusText\":\"Unauthorized\",\"errorCode\":3010,\"payload\":\"Invalid\n      username or password\"}'}\n  - {url: 'https://api.empatica.com/v2/users/me', method: GET, auth: none, http_status: 401,\n    response: '{\"status\":\"Missing token\",\"statusText\":\"\",\"errorCode\":3998}'}\n  - {url: 'https://api.empatica.com/v2/users/me', method: GET, auth: 'Bearer <invalid>',\n    http_status: 401, response: '{\"status\":\"Missing token\",\"statusText\":\"\",\"errorCode\":3998}'}\n  - {url:\
  \ 'https://api.empatica.com/v2/devices', method: POST, auth: none, http_status: 401,\n    response: '{\"status\":\"Missing token\",\"statusText\":\"\",\"errorCode\":3998}'}\n  cors_advertised_headers:\n  - origin\n  - x-requested-with\n  - content-type\n  - accept\n  - authorization\n  - x-emp-app-version\n  - x-emp-app-name\n  - x-emp-app-platform\n  - x-forwarded-for\n  - elastic-apm-traceparent\n- id: cloud-api-credentials\n  applies_to: empatica-cloud-api\n  type: unknown\n  method: none\n  documented: false\n  description: >-\n    The Cloud API's authentication model is not published. Empatica states on\n    https://www.empatica.com/cloud-api/ that \"All Cloud API clients will be\n    provided with full developer documentation\", so the auth scheme is disclosed\n    only after a contract is in place. Recorded as unknown rather than guessed.\n  x-evidence:\n  - {url: 'https://www.empatica.com/cloud-api/', http_status: 200, finding: no auth\n      scheme, base URL or reference published}\n\
  oauth2: false\nopenid_connect: false\nmutual_tls: not-documented\nmfa: not-documented\ngaps:\n- No public API reference documents any authentication scheme for the Cloud API.\n- No OAuth 2.0 or OIDC discovery document is served on any Empatica host.\n- api.empatica.com returns no WWW-Authenticate header on a 401, so a client cannot\n  discover the scheme from the challenge.\n- Data Access Keys cap at two active sets with no overlap window, which forces a\n  break-then-rotate posture for automated consumers.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/empatica/refs/heads/main/authentication/empatica-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Healthcare
- Digital Health
- Wearables
- Medical Devices
- Clinical Trials
- Remote Patient Monitoring
- Digital Biomarkers
- Life Sciences
- Sensor Data
---
