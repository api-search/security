---
anonymous_access: false
api_key_in: []
api_specs:
- filename: korala-ai-billing-api-openapi.yml
  format: yaml
  label: Korala AI Billing API
  slug: korala-ai-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/korala-ai/openapi/korala-ai-billing-api-openapi.yml
- filename: korala-ai-catalog-api-openapi.yml
  format: yaml
  label: Korala AI Catalog API
  slug: korala-ai-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/korala-ai/openapi/korala-ai-catalog-api-openapi.yml
- filename: korala-ai-collections-api-openapi.yml
  format: yaml
  label: Korala AI Collections API
  slug: korala-ai-collections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/korala-ai/openapi/korala-ai-collections-api-openapi.yml
- filename: korala-ai-documents-api-openapi.yml
  format: yaml
  label: Korala AI Documents API
  slug: korala-ai-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/korala-ai/openapi/korala-ai-documents-api-openapi.yml
- filename: korala-ai-field-detection-api-openapi.yml
  format: yaml
  label: Korala AI Field Detection API
  slug: korala-ai-field-detection-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/korala-ai/openapi/korala-ai-field-detection-api-openapi.yml
- filename: korala-ai-google-workspace-api-openapi.yml
  format: yaml
  label: Korala AI Google Workspace API
  slug: korala-ai-google-workspace-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/korala-ai/openapi/korala-ai-google-workspace-api-openapi.yml
- filename: korala-ai-public-workflows-api-openapi.yml
  format: yaml
  label: Korala AI Public Workflows API
  slug: korala-ai-public-workflows-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/korala-ai/openapi/korala-ai-public-workflows-api-openapi.yml
- filename: korala-ai-risk-api-openapi.yml
  format: yaml
  label: Korala AI Risk API
  slug: korala-ai-risk-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/korala-ai/openapi/korala-ai-risk-api-openapi.yml
- filename: korala-ai-screening-api-openapi.yml
  format: yaml
  label: Korala AI Screening API
  slug: korala-ai-screening-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/korala-ai/openapi/korala-ai-screening-api-openapi.yml
- filename: korala-ai-session-access-api-openapi.yml
  format: yaml
  label: Korala AI Session Access API
  slug: korala-ai-session-access-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/korala-ai/openapi/korala-ai-session-access-api-openapi.yml
- filename: korala-ai-session-configurations-api-openapi.yml
  format: yaml
  label: Korala AI Session Configurations API
  slug: korala-ai-session-configurations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/korala-ai/openapi/korala-ai-session-configurations-api-openapi.yml
- filename: korala-ai-sessions-api-openapi.yml
  format: yaml
  label: Korala AI Sessions API
  slug: korala-ai-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/korala-ai/openapi/korala-ai-sessions-api-openapi.yml
- filename: korala-ai-signatures-api-openapi.yml
  format: yaml
  label: Korala AI Signatures API
  slug: korala-ai-signatures-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/korala-ai/openapi/korala-ai-signatures-api-openapi.yml
- filename: korala-ai-signing-packets-api-openapi.yml
  format: yaml
  label: Korala AI Signing Packets API
  slug: korala-ai-signing-packets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/korala-ai/openapi/korala-ai-signing-packets-api-openapi.yml
- filename: korala-ai-template-field-detection-api-openapi.yml
  format: yaml
  label: Korala AI Template Field Detection API
  slug: korala-ai-template-field-detection-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/korala-ai/openapi/korala-ai-template-field-detection-api-openapi.yml
- filename: korala-ai-template-preparation-api-openapi.yml
  format: yaml
  label: Korala AI Template Preparation API
  slug: korala-ai-template-preparation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/korala-ai/openapi/korala-ai-template-preparation-api-openapi.yml
- filename: korala-ai-template-preparation-browser-api-openapi.yml
  format: yaml
  label: Korala AI Template Preparation Browser API
  slug: korala-ai-template-preparation-browser-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/korala-ai/openapi/korala-ai-template-preparation-browser-api-openapi.yml
- filename: korala-ai-templates-api-openapi.yml
  format: yaml
  label: Korala AI Templates API
  slug: korala-ai-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/korala-ai/openapi/korala-ai-templates-api-openapi.yml
- filename: korala-ai-webhooks-api-openapi.yml
  format: yaml
  label: Korala AI Webhooks API
  slug: korala-ai-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/korala-ai/openapi/korala-ai-webhooks-api-openapi.yml
- filename: korala-ai-workflows-api-openapi.yml
  format: yaml
  label: Korala AI Workflows API
  slug: korala-ai-workflows-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/korala-ai/openapi/korala-ai-workflows-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Korala AI Authentication
name_suffix: Authentication
oauth_flows: []
overview: Korala AI declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Korala AI
provider_slug: korala-ai
scheme_count: 3
schemes:
- evidence: Korala secures API requests with HMAC-SHA256 signatures.
  header: X-API-Key
  how_to_obtain: Create an API key in Korala under Settings → API Keys.
  location: header
  name: HMAC-SHA256
  type: hmac
- evidence: Korala secures API requests with HMAC-SHA256 signatures.
  header: X-Timestamp
  how_to_obtain: Create an API key in Korala under Settings → API Keys.
  location: header
  name: HMAC-SHA256
  type: hmac
- evidence: Korala secures API requests with HMAC-SHA256 signatures.
  header: X-Signature
  how_to_obtain: Create an API key in Korala under Settings → API Keys.
  location: header
  name: HMAC-SHA256
  type: hmac
slug: korala-ai-authentication
source_filename: korala-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.korala.ai/guides/authentication
source_yaml: "generated: '2026-11-14'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.korala.ai/guides/authentication\nsources:\n- https://docs.korala.ai/guides/authentication\n- https://docs.korala.ai/ai-agents/api-key\n- https://docs.korala.ai/guides/signing-quickstart\n- https://docs.korala.ai/guides/signing-packets\nschemes:\n- type: hmac\n  name: HMAC-SHA256\n  evidence: Korala secures API requests with HMAC-SHA256 signatures.\n  location: header\n  header: X-API-Key\n  how_to_obtain: Create an API key in Korala under Settings → API Keys.\n- type: hmac\n  name: HMAC-SHA256\n  evidence: Korala secures API requests with HMAC-SHA256 signatures.\n  location: header\n  header: X-Timestamp\n  how_to_obtain: Create an API key in Korala under Settings → API Keys.\n- type: hmac\n  name: HMAC-SHA256\n  evidence: Korala secures API requests with HMAC-SHA256 signatures.\n  location: header\n  header: X-Signature\n  how_to_obtain: Create an API key in Korala\
  \ under Settings → API Keys.\ndocs: https://docs.korala.ai/guides/authentication\n"
source_yaml_url: https://artifacts.apis.io/korala-ai/authentication/korala-ai-authentication.yml
summary_line: 3 schemes
tags:
- Identity
- Fraud Prevention
- E-Signature
- Artificial Intelligence
---
