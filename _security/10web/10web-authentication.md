---
api_key_in: []
api_specs:
- filename: 10web-account-api-openapi.yml
  format: yaml
  label: 10Web Account API
  slug: 10web-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/10web/refs/heads/main/openapi/10web-account-api-openapi.yml
- filename: 10web-backup-api-openapi.yml
  format: yaml
  label: 10Web Backup API
  slug: 10web-backup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/10web/refs/heads/main/openapi/10web-backup-api-openapi.yml
- filename: 10web-builder-api-openapi.yml
  format: yaml
  label: 10Web Builder API
  slug: 10web-builder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/10web/refs/heads/main/openapi/10web-builder-api-openapi.yml
- filename: 10web-cache-api-openapi.yml
  format: yaml
  label: 10Web Cache API
  slug: 10web-cache-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/10web/refs/heads/main/openapi/10web-cache-api-openapi.yml
- filename: 10web-certificate-api-openapi.yml
  format: yaml
  label: 10Web Certificate API
  slug: 10web-certificate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/10web/refs/heads/main/openapi/10web-certificate-api-openapi.yml
- filename: 10web-domain-api-openapi.yml
  format: yaml
  label: 10Web Domain API
  slug: 10web-domain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/10web/refs/heads/main/openapi/10web-domain-api-openapi.yml
- filename: 10web-php-management-api-openapi.yml
  format: yaml
  label: 10Web PHP Management API
  slug: 10web-php-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/10web/refs/heads/main/openapi/10web-php-management-api-openapi.yml
- filename: 10web-section-based-ai-api-openapi.yml
  format: yaml
  label: 10Web Section Based AI API
  slug: 10web-section-based-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/10web/refs/heads/main/openapi/10web-section-based-ai-api-openapi.yml
- filename: 10web-subdomain-api-openapi.yml
  format: yaml
  label: 10Web Subdomain API
  slug: 10web-subdomain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/10web/refs/heads/main/openapi/10web-subdomain-api-openapi.yml
- filename: 10web-vibe-coding-api-openapi.yml
  format: yaml
  label: 10Web Vibe Coding API
  slug: 10web-vibe-coding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/10web/refs/heads/main/openapi/10web-vibe-coding-api-openapi.yml
- filename: 10web-website-api-openapi.yml
  format: yaml
  label: 10Web Website API
  slug: 10web-website-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/10web/refs/heads/main/openapi/10web-website-api-openapi.yml
- filename: 10web-wp-autologin-api-openapi.yml
  format: yaml
  label: 10Web WP Autologin API
  slug: 10web-wp-autologin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/10web/refs/heads/main/openapi/10web-wp-autologin-api-openapi.yml
- filename: 10web-zone-api-openapi.yml
  format: yaml
  label: 10Web Zone API
  slug: 10web-zone-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/10web/refs/heads/main/openapi/10web-zone-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: 10Web Authentication
name_suffix: Authentication
oauth_flows: []
overview: 10Web declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: 10Web
provider_slug: 10web
scheme_count: 1
schemes:
- applies_to: all operations
  description: API key for authentication. Passed as the x-api-key request header on every call to https://api.10web.io. Obtain the key from the 10Web Reseller Dashboard. Missing or invalid keys return HTTP 401 with {"status":"error","message":"Unauthorized access"}.
  id: api-key
  in: header
  name: x-api-key
  required: true
  type: apiKey
slug: 10web-authentication
source_filename: 10web-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://apidocs.10web.io/ (OpenAPI Authorization parameter) + https://help.10web.io/hc/en-us/articles/27304964365586-Introduction-to-10Web-API\napi: 10Web API V1\nsummary: >-\n  The 10Web API authenticates every request with a static API key sent in the\n  x-api-key HTTP request header. Reseller/partner API keys are issued from the\n  10Web Dashboard. Webhook deliveries are separately verified with an HMAC-SHA256\n  signature computed from a per-endpoint webhook secret (whsec_ prefix).\nschemes:\n- id: api-key\n  type: apiKey\n  in: header\n  name: x-api-key\n  required: true\n  description: >-\n    API key for authentication. Passed as the x-api-key request header on every\n    call to https://api.10web.io. Obtain the key from the 10Web Reseller\n    Dashboard. Missing or invalid keys return HTTP 401 with\n    {\"status\":\"error\",\"message\":\"Unauthorized access\"}.\n  applies_to: all operations\nwebhook_verification:\n\
  \  method: HMAC-SHA256\n  header: x-10web-signature\n  format: 'v1=HMAC_SHA256_HEX(webhook_secret, timestamp + \".\" + raw_body)'\n  secret_prefix: whsec_\n  note: >-\n    Webhook signatures use the per-endpoint webhook secret (not the API key).\n    The secret is generated on first save of a webhook URL in the dashboard.\nnotes:\n- No OAuth 2.0 / OpenID Connect flow is documented; the API uses a single static\n  API-key credential.\n- The OpenAPI document declares the credential as a shared header parameter\n  (components.parameters.Authorization -> name x-api-key) rather than a formal\n  securityScheme, so it is captured here from the spec + docs.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/10web/refs/heads/main/authentication/10web-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Artificial Intelligence
- Website Builder
- WordPress
- Hosting
- Website Generation
- No-Code
---
