---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Optinmonster Authentication
name_suffix: Authentication
oauth_flows: []
overview: OptinMonster declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: OptinMonster
provider_slug: optinmonster
scheme_count: 0
schemes: []
slug: optinmonster-authentication
source_filename: optinmonster-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: >-\n  https://optinmonster.com/docs/how-the-optinmonster-api-key-works-with-wordpress/ ;\n  https://plugins.svn.wordpress.org/optinmonster/trunk/OMAPI/Api.php ;\n  live OPTIONS preflight against https://api.optinmonster.com/v2/campaigns\ndocs: https://optinmonster.com/docs/how-the-optinmonster-api-key-works-with-wordpress/\nnote: >-\n  OptinMonster publishes no OpenAPI, so this profile is assembled from three real sources: the\n  help-center API-key article, the first-party WordPress plugin source (OMAPI/Api.php, which builds\n  every request the vendor's own client makes), and a live CORS preflight whose\n  `access-control-allow-headers` enumerates every credential header the API accepts. There is no\n  OAuth 2.0 and no OpenID Connect surface anywhere on the platform — key auth only — so no\n  scopes/ artifact is emitted.\nsummary:\n  schemes: 2\n  primary: api-key-header\n  oauth2: false\n  openid_connect: false\n  mtls:\
  \ false\n  scopes: false\nsecuritySchemes:\n- id: apiKeyHeader\n  type: apiKey\n  in: header\n  name: X-OptinMonster-ApiKey\n  primary: true\n  description: >-\n    The account API key, issued in the OptinMonster app under My Account > API. Sent on every\n    request as the `X-OptinMonster-ApiKey` header. The API may also return this header on a\n    response, which the WordPress plugin captures to upgrade a legacy credential pair to a key.\n  evidence:\n  - source: plugin-source\n    detail: \"OMAPI/Api.php line 260: $headers['X-OptinMonster-ApiKey'] = $this->apikey;\"\n    url: https://plugins.svn.wordpress.org/optinmonster/trunk/OMAPI/Api.php\n  - source: cors-preflight\n    detail: >-\n      OPTIONS https://api.optinmonster.com/v2/campaigns returns\n      access-control-allow-headers including X-OptinMonster-ApiKey\n    http_status: 200\n- id: legacyKeyUser\n  type: apiKey\n  in: query\n  name: omapi-key\n  primary: false\n  deprecated: true\n  description: >-\n    The legacy credential\
  \ pair — an API key plus an API username — carried as `omapi-key` (and a\n    paired user value) in the request body/query rather than as a header. Still accepted, but the\n    help-center article states an API key is no longer required to connect the WordPress plugin,\n    and the plugin migrates a legacy pair to the header key on first successful call.\n  evidence:\n  - source: plugin-source\n    detail: \"OMAPI/Api.php line 223: 'omapi-key' => $this->key\"\n    url: https://plugins.svn.wordpress.org/optinmonster/trunk/OMAPI/Api.php\naccepted_auth_headers:\n  note: >-\n    Read verbatim from the live `access-control-allow-headers` on an OPTIONS preflight. Presence in\n    this list means the edge will accept the header cross-origin; it does not prove every one is an\n    active credential path. X-OptinMonster-ApiKey is the one the vendor's own client uses.\n  observed:\n  - X-OptinMonster-ApiKey\n  - X-OptinMonster-SKey\n  - Bearer-Token\n  - X-Auth-Token\n  - Authorization\n  - Auth\n\
  \  - X-CSRF-Token\n  - X-XSRF-Token\n  fetched: '2026-08-12'\n  url: https://api.optinmonster.com/v2/campaigns\n  http_status: 200\ncontext_headers:\n  note: >-\n    Not credentials — identification/telemetry headers the first-party WordPress client sends\n    alongside the key, and which the edge explicitly allows.\n  headers:\n  - name: OMAPI-Referer\n    value: the calling site URL\n  - name: OMAPI-Sender\n    value: WordPress\n  - name: OMAPI-Site\n    value: the WordPress blog name\n  - name: OMAPI-Version\n    value: the plugin version\n  - name: OMAPI-Plugins\n    value: active-plugin fingerprint\n  - name: X-OptinMonster-UrlPath\n  - name: X-OptinMonster-Campaigns\n  - name: X-SC-Touchpoint\nunauthenticated_surface:\n- path: /v2/templates\n  method: GET\n  http_status: 200\n  description: >-\n    The campaign template catalog is served without any credential — 697 template objects,\n    1.27 MB, on 2026-08-12. The only anonymous data endpoint found.\n  fetched: '2026-08-12'\nkey_management:\n\
  \  issue: https://app.optinmonster.com/ (My Account > API)\n  rotate: >-\n    POST v2/key/regenerate — the plugin calls this to regenerate the account key.\n  revoke: undocumented publicly\nwebhook_auth:\n  supported: false\n  note: >-\n    Outbound webhooks carry no authentication. The docs state verbatim \"At this time we do not\n    support Authentication for Webhook.\" Receivers must validate by other means.\n  source: https://optinmonster.com/docs/how-to-connect-optinmonster-with-a-webhook/\ngaps:\n- No OpenAPI or public API reference documents the authentication scheme; the header name is\n  discoverable only from the plugin source or a CORS preflight.\n- No OAuth 2.0, so no delegated/third-party authorization and no scope model.\n- Webhook deliveries are unauthenticated and unsigned.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/optinmonster/refs/heads/main/authentication/optinmonster-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Lead Generation
- Marketing
- Conversion Optimization
- Email Marketing
- Popups
- WordPress
- Webhooks
- SaaS
- Marketing Automation
---
