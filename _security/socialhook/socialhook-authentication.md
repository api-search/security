---
anonymous_access: false
api_key_in: []
api_specs:
- filename: socialhook-openapi-generated.yml
  format: yaml
  label: Lead Lock Systems API
  slug: socialhook-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/socialhook/openapi/_ae-authored/socialhook-openapi-generated.yml
auth_types: []
description: Authentication is performed by verifying an HMAC‑SHA256 signature sent in a request header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Socialhook Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lead Lock Systems declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Lead Lock Systems
provider_slug: socialhook
scheme_count: 1
schemes:
- evidence: This hash is sent in the X-SocialHook-Signature HTTP header in the format sha256=<hex_digest> .
  header: X-SocialHook-Signature
  how_to_obtain: Generate a secret key in the SocialHook dashboard; the key is used to compute the HMAC‑SHA256 signature for each payload.
  location: header
  name: X-SocialHook-Signature
  type: apiKey
slug: socialhook-authentication
source_filename: socialhook-authentication.yml
source_heading: Authentication Profile
source_url: https://socialhook.io/en/security
source_yaml: "generated: '2026-10-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://socialhook.io/en/security\nsources:\n- https://socialhook.io/en/security\n- https://socialhook.io/en/docs/quickstart\n- https://socialhook.io/en/blog/whatsapp-webhook-setup-reference\n- https://socialhook.io/en/blog/whatsapp-chatbot-ecommerce\ndescription: Authentication is performed by verifying an HMAC‑SHA256 signature sent in a request header.\nschemes:\n- type: apiKey\n  name: X-SocialHook-Signature\n  evidence: This hash is sent in the X-SocialHook-Signature HTTP header in the format sha256=<hex_digest> .\n  location: header\n  header: X-SocialHook-Signature\n  how_to_obtain: Generate a secret key in the SocialHook dashboard; the key is used to compute the HMAC‑SHA256 signature for each payload.\nnote: No OAuth2, HTTP basic, bearer, JWT, HMAC, MTLS, or other authentication schemes are documented.\ndocs: https://socialhook.io/en/security\n"
source_yaml_url: https://artifacts.apis.io/socialhook/authentication/socialhook-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Webhook
- Social Media
- Integration
- Automation
---
