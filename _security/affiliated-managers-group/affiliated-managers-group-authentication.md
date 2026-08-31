---
api_key_in: []
api_specs:
- filename: affiliated-managers-group-funds-data-openapi.yml
  format: yaml
  label: AMG Funds Data API
  slug: affiliated-managers-group-funds-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affiliated-managers-group/refs/heads/main/openapi/affiliated-managers-group-funds-data-openapi.yml
- filename: affiliated-managers-group-corporate-openapi.yml
  format: yaml
  label: AMG Corporate Content API
  slug: affiliated-managers-group-corporate-content
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affiliated-managers-group/refs/heads/main/openapi/affiliated-managers-group-corporate-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Affiliated Managers Group Authentication
name_suffix: Authentication
oauth_flows: []
overview: Affiliated Managers Group declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Affiliated Managers Group
provider_slug: affiliated-managers-group
scheme_count: 0
schemes: []
slug: affiliated-managers-group-authentication
source_filename: affiliated-managers-group-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: probed\nsource: >-\n  live anonymous requests against https://wealth.amg.com/wp-json/amgfundsdata/v1/* and\n  https://www.amg.com/wp-json/amginc/v1/affiliates on 2026-08-30, plus the WordPress REST discovery\n  documents at https://wealth.amg.com/wp-json/ and https://www.amg.com/wp-json/\nprovider: Affiliated Managers Group\nproviderId: affiliated-managers-group\nsummary: >-\n  Both AMG site-backing APIs answer anonymously. No API key, bearer token, OAuth flow or signed\n  request is required or accepted for read access, and neither derived OpenAPI declares a\n  securityScheme because the provider's route table declares none. The only credential surface either\n  WordPress host advertises is application passwords for wp-admin, which is a CMS administration\n  mechanism for AMG staff, not a consumer-facing API credential.\napis:\n  - name: AMG Funds Data API\n    host: wealth.amg.com\n    base: https://wealth.amg.com/wp-json/amgfundsdata/v1\n\
  \    authentication:\n      required: false\n      schemes: []\n      evidence:\n        - url: https://wealth.amg.com/wp-json/amgfundsdata/v1/products/funds\n          method: GET\n          headers_sent: none\n          status: 200\n          content_type: application/json\n        - url: https://wealth.amg.com/wp-json/amgfundsdata/v1/fund-detail/BBAIX/overview\n          method: GET\n          headers_sent: none\n          status: 200\n          content_type: application/json\n  - name: AMG Corporate Content API\n    host: www.amg.com\n    base: https://www.amg.com/wp-json/amginc/v1\n    authentication:\n      required: false\n      schemes: []\n      evidence:\n        - url: https://www.amg.com/wp-json/amginc/v1/affiliates\n          method: POST\n          body: '{}'\n          headers_sent: 'Content-Type: application/json'\n          status: 200\n          content_type: application/json\nadmin_credential_surface:\n  mechanism: WordPress application passwords\n  scope: site administration\
  \ only — not a consumer API credential\n  authorization_endpoints:\n    - https://www.amg.com/wp-admin/authorize-application.php\n    - https://wealth.amg.com/wp-admin/authorize-application.php\n  source: the `authentication` block of each host's /wp-json/ discovery document\noauth:\n  supported: false\n  evidence:\n    - url: https://www.amg.com/.well-known/oauth-authorization-server\n      status: 404\n    - url: https://wealth.amg.com/.well-known/oauth-authorization-server\n      status: 404\n    - url: https://www.amg.com/.well-known/openid-configuration\n      status: 404\ncaveats: >-\n  Anonymous read access is what the provider currently serves; it is not a documented guarantee. AMG\n  publishes no developer terms covering programmatic use of these endpoints, so access could change\n  without notice and consumers have no support channel or contractual position.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/affiliated-managers-group/refs/heads/main/authentication/affiliated-managers-group-authentication.yml
summary_line: 0 schemes
tags:
- Asset Management
- Investment Management
- Financial-Services
- Wealth Management
- Institutional Investing
- Fortune 1000
---
