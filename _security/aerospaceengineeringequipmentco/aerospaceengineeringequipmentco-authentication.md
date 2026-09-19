---
anonymous_access: false
api_key_in: []
api_specs:
- filename: aerospaceengineeringequipmentco-products-api-openapi.yml
  format: yaml
  label: AEE Products API
  slug: aee-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aerospaceengineeringequipmentco/refs/heads/main/openapi/aerospaceengineeringequipmentco-products-api-openapi.yml
- filename: aerospaceengineeringequipmentco-categories-api-openapi.yml
  format: yaml
  label: Aerospace Engineering Equipment Categories API
  slug: aerospaceengineeringequipmentco-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aerospaceengineeringequipmentco/refs/heads/main/openapi/aerospaceengineeringequipmentco-categories-api-openapi.yml
- filename: aerospaceengineeringequipmentco-media-api-openapi.yml
  format: yaml
  label: Aerospace Engineering Equipment Media API
  slug: aerospaceengineeringequipmentco-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aerospaceengineeringequipmentco/refs/heads/main/openapi/aerospaceengineeringequipmentco-media-api-openapi.yml
- filename: aerospaceengineeringequipmentco-pages-api-openapi.yml
  format: yaml
  label: Aerospace Engineering Equipment Pages API
  slug: aerospaceengineeringequipmentco-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aerospaceengineeringequipmentco/refs/heads/main/openapi/aerospaceengineeringequipmentco-pages-api-openapi.yml
- filename: aerospaceengineeringequipmentco-posts-api-openapi.yml
  format: yaml
  label: Aerospace Engineering Equipment Posts API
  slug: aerospaceengineeringequipmentco-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aerospaceengineeringequipmentco/refs/heads/main/openapi/aerospaceengineeringequipmentco-posts-api-openapi.yml
- filename: aerospaceengineeringequipmentco-product-categories-api-openapi.yml
  format: yaml
  label: Aerospace Engineering Equipment Product Categories API
  slug: aerospaceengineeringequipmentco-product-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aerospaceengineeringequipmentco/refs/heads/main/openapi/aerospaceengineeringequipmentco-product-categories-api-openapi.yml
- filename: aerospaceengineeringequipmentco-registries-api-openapi.yml
  format: yaml
  label: Aerospace Engineering Equipment Registries API
  slug: aerospaceengineeringequipmentco-registries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aerospaceengineeringequipmentco/refs/heads/main/openapi/aerospaceengineeringequipmentco-registries-api-openapi.yml
- filename: aerospaceengineeringequipmentco-search-api-openapi.yml
  format: yaml
  label: Aerospace Engineering Equipment Search API
  slug: aerospaceengineeringequipmentco-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aerospaceengineeringequipmentco/refs/heads/main/openapi/aerospaceengineeringequipmentco-search-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: probed
name: Aerospaceengineeringequipmentco Authentication
name_suffix: Authentication
oauth_flows: []
overview: Aerospace Engineering Equipment declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Aerospace Engineering Equipment
provider_slug: aerospaceengineeringequipmentco
scheme_count: 0
schemes: []
slug: aerospaceengineeringequipmentco-authentication
source_filename: aerospaceengineeringequipmentco-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-10'\nmethod: probed\nsource: >-\n  https://a-fsw.com/wp-json/ (route index, authentication block) plus live anonymous and context=edit\n  probes of the wp/v2 routes on 2026-09-10\nsummary: >-\n  The public AEE surface requires no authentication and offers no credential of any kind: every route\n  documented in openapi/ answers HTTP 200 to an anonymous GET in the default context=view. There is no\n  developer program, no key issuance, no OAuth and no signup. The only authentication mechanism the server\n  advertises is WordPress application passwords, which gate the write methods and the privileged read\n  contexts; those are administrator surfaces, not a published API product.\npublic_surface:\n  authentication_required: false\n  verified: '2026-09-10'\n  evidence:\n  - {url: 'https://a-fsw.com/wp-json/wp/v2/product?per_page=1', status: 200, note: 'Anonymous GET returns published products.'}\n  - {url: 'https://a-fsw.com/wp-json/wp/v2/posts?per_page=1',\
  \ status: 200, note: 'Anonymous GET returns published posts.'}\nsecurity_schemes: []\nschemes_advertised_but_not_public:\n- id: application-passwords\n  type: http\n  scheme: basic\n  standard: WordPress application passwords (HTTP Basic with a generated per-application password)\n  authorization_endpoint: https://a-fsw.com/wp-admin/authorize-application.php\n  source: 'https://a-fsw.com/wp-json/ -> authentication.application-passwords.endpoints.authorization'\n  applies_to: >-\n    Write methods (POST/PUT/PATCH/DELETE) on wp/v2 routes, the privileged read context=edit, and the\n    administrative namespaces (wp-abilities/v1, fluentform/v1, spc/v1, google-site-kit/v1, wp-site-health/v1).\n  public: false\n  note: >-\n    This is WordPress core administration, not an AEE API product. It is recorded because the server\n    advertises it in its own route index, and because it is the reason the write half of every documented\n    route is deliberately absent from openapi/.\ngated_probes:\n\
  - {url: 'https://a-fsw.com/wp-json/wp/v2/product?context=edit', status: 401, code: rest_forbidden_context, note: 'Privileged read context refused anonymously.'}\n- {url: 'https://a-fsw.com/wp-json/wp/v2/settings', status: 401, code: rest_forbidden}\n- {url: 'https://a-fsw.com/wp-json/wp-abilities/v1/abilities', status: 401, code: rest_forbidden, note: 'The WordPress Abilities API — the agent-facing tool registry — is installed but auth-gated. No anonymous tool discovery is possible.'}\n- {url: 'https://a-fsw.com/wp-json/fluentform/v1/forms/ping', status: 401, code: rest_forbidden}\noauth:\n  present: false\n  note: 'No oauth2 or openIdConnect scheme is declared or served; /.well-known/openid-configuration and /.well-known/oauth-authorization-server both 404. No scopes/ artifact is emitted.'\ndocs: null\ndocs_note: 'AEE publishes no authentication documentation because it publishes no developer program.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aerospaceengineeringequipmentco/refs/heads/main/authentication/aerospaceengineeringequipmentco-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Manufacturing
- Industrial Equipment
- Welding
- Friction Stir Welding
- Aerospace
- Rail Transit
- Automotive
- Shipbuilding
- Content
- China
---
