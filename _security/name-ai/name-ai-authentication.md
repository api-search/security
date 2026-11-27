---
anonymous_access: false
api_key_in: []
api_specs:
- filename: name-ai-batch-api-openapi.yml
  format: yaml
  label: Name.ai Batch API
  slug: name-ai-batch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/name-ai/openapi/name-ai-batch-api-openapi.yml
- filename: name-ai-domain-api-openapi.yml
  format: yaml
  label: Name.ai Domain API
  slug: name-ai-domain-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/name-ai/openapi/name-ai-domain-api-openapi.yml
- filename: name-ai-domains-api-openapi.yml
  format: yaml
  label: Name.ai Domains API
  slug: name-ai-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/name-ai/openapi/name-ai-domains-api-openapi.yml
- filename: name-ai-market-api-openapi.yml
  format: yaml
  label: Name.ai Market API
  slug: name-ai-market-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/name-ai/openapi/name-ai-market-api-openapi.yml
- filename: name-ai-pricing-api-openapi.yml
  format: yaml
  label: Name.ai Pricing API
  slug: name-ai-pricing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/name-ai/openapi/name-ai-pricing-api-openapi.yml
- filename: name-ai-tlds-api-openapi.yml
  format: yaml
  label: Name.ai Tlds API
  slug: name-ai-tlds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/name-ai/openapi/name-ai-tlds-api-openapi.yml
- filename: name-ai-tools-api-openapi.yml
  format: yaml
  label: Name.ai Tools API
  slug: name-ai-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/name-ai/openapi/name-ai-tools-api-openapi.yml
auth_types: []
description: Authentication schemes for Name.ai APIs
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Name.ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Name.ai declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Name.ai
provider_slug: name-ai
scheme_count: 2
schemes:
- authorize_url: https://name.ai/oauth/authorize
  evidence: The scheme is OAuth 2.1, authorization_code with PKCE (S256), public clients only.
  flows:
  - authorization_code
  header: Authorization
  how_to_obtain: Dynamic client registration (POST https://name.ai/api/oauth/register) returns a client_id; then use the authorization endpoint with PKCE to obtain an authorization code and exchange it at the token endpoint (POST https://name.ai/api/oauth/token) for an access token.
  location: header
  name: OAuth 2.1
  scopes:
  - pricing:read
  type: oauth2
- evidence: Secure every Partner API request by signing it from your backend with your API secret.
  how_to_obtain: Obtain an API secret (sk_*) and a public key id (pk_*) from the Name.ai Partner program; then include the required HMAC headers (X-NameAI-Key-Id, X-NameAI-Timestamp, X-NameAI-Nonce, X-NameAI-Signature) on each request.
  location: header
  name: HMAC authentication
  type: hmac
slug: name-ai-authentication
source_filename: name-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://name.ai/developers/auth
source_yaml: "generated: '2026-11-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://name.ai/developers/auth\nsources:\n- https://name.ai/developers/auth\n- https://name.ai/partners/docs/authentication\n- https://name.ai/auth.md\ndescription: Authentication schemes for Name.ai APIs\nschemes:\n- type: oauth2\n  name: OAuth 2.1\n  evidence: The scheme is OAuth 2.1, authorization_code with PKCE (S256), public clients only.\n  location: header\n  header: Authorization\n  flows:\n  - authorization_code\n  authorize_url: https://name.ai/oauth/authorize\n  scopes:\n  - pricing:read\n  how_to_obtain: Dynamic client registration (POST https://name.ai/api/oauth/register) returns a client_id; then use the authorization endpoint\n    with PKCE to obtain an authorization code and exchange it at the token endpoint (POST https://name.ai/api/oauth/token) for an access token.\n- type: hmac\n  name: HMAC authentication\n  evidence: Secure every Partner API request by signing\
  \ it from your backend with your API secret.\n  location: header\n  how_to_obtain: Obtain an API secret (sk_*) and a public key id (pk_*) from the Name.ai Partner program; then include the required HMAC headers\n    (X-NameAI-Key-Id, X-NameAI-Timestamp, X-NameAI-Nonce, X-NameAI-Signature) on each request.\ndocs: https://name.ai/developers/auth\n"
source_yaml_url: https://artifacts.apis.io/name-ai/authentication/name-ai-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Artificial Intelligence
- Domain
- Marketplace
- Software-as-a-Service
---
