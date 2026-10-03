---
anonymous_access: false
api_key_in: []
api_specs:
- filename: asapp3-autocompose-api-openapi.yml
  format: yaml
  label: Asapp3 Auto Compose API
  slug: asapp3-autocompose-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asapp3/refs/heads/main/openapi/asapp3-autocompose-api-openapi.yml
- filename: asapp3-autosummary-api-openapi.yml
  format: yaml
  label: Asapp3 Auto Summary API
  slug: asapp3-autosummary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asapp3/refs/heads/main/openapi/asapp3-autosummary-api-openapi.yml
- filename: asapp3-autotranscribe-api-openapi.yml
  format: yaml
  label: Asapp3 Auto Transcribe API
  slug: asapp3-autotranscribe-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asapp3/refs/heads/main/openapi/asapp3-autotranscribe-api-openapi.yml
- filename: asapp3-autotranscribe-media-gateway-api-openapi.yml
  format: yaml
  label: Asapp3 AutoTranscribe Media Gateway API
  slug: asapp3-autotranscribe-media-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asapp3/refs/heads/main/openapi/asapp3-autotranscribe-media-gateway-api-openapi.yml
- filename: asapp3-conversations-api-openapi.yml
  format: yaml
  label: Asapp3 Conversations API
  slug: asapp3-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asapp3/refs/heads/main/openapi/asapp3-conversations-api-openapi.yml
- filename: asapp3-file-exporter-api-openapi.yml
  format: yaml
  label: Asapp3 File Exporter API
  slug: asapp3-file-exporter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asapp3/refs/heads/main/openapi/asapp3-file-exporter-api-openapi.yml
- filename: asapp3-generativeagent-api-openapi.yml
  format: yaml
  label: Asapp3 Generative Agent API
  slug: asapp3-generativeagent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asapp3/refs/heads/main/openapi/asapp3-generativeagent-api-openapi.yml
- filename: asapp3-health-check-api-openapi.yml
  format: yaml
  label: Asapp3 Health Check API
  slug: asapp3-health-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asapp3/refs/heads/main/openapi/asapp3-health-check-api-openapi.yml
- filename: asapp3-knowledge-base-api-openapi.yml
  format: yaml
  label: Asapp3 Knowledge Base API
  slug: asapp3-knowledge-base-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asapp3/refs/heads/main/openapi/asapp3-knowledge-base-api-openapi.yml
- filename: asapp3-metadata-api-openapi.yml
  format: yaml
  label: Asapp3 Metadata API
  slug: asapp3-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asapp3/refs/heads/main/openapi/asapp3-metadata-api-openapi.yml
auth_types: []
description: Authentication methods documented for ASAPP web SDK, API connections, and mobile SDKs.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Asapp3 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Asapp3 declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Asapp3
provider_slug: asapp3
scheme_count: 2
schemes:
- evidence: Custom headers add authentication data to API requests via HTTP headers. Common implementations include API keys and bearer tokens.
  how_to_obtain: Configure a header name (e.g., "Authorization" or "X-API-Key") and a static or dynamic header value in the API connection settings.
  name: Custom Header Authentication
  type: apiKey
- evidence: The request context provider is a function that returns a map with keys and values agreed upon with ASAPP.
  how_to_obtain: Implement ASAPPRequestContextProvider that returns an Auth map containing a Token.
  name: Android SDK – Request Context Provider
  type: other
slug: asapp3-authentication
source_filename: asapp3-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.asapp.com/generativeagent/integrate/web-sdk/web-authentication.md
source_yaml: "generated: '2026-09-26'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.asapp.com/generativeagent/integrate/web-sdk/web-authentication.md\nsources:\n- https://docs.asapp.com/generativeagent/integrate/web-sdk/web-authentication.md\n- https://docs.asapp.com/generativeagent/configuring/connect-apis/authentication-methods.md\n- https://docs.asapp.com/agent-desk/integrations/android-sdk/user-authentication.md\n- https://docs.asapp.com/agent-desk/integrations/customer-authentication.md\ndescription: Authentication methods documented for ASAPP web SDK, API connections, and mobile SDKs.\nschemes:\n- type: apiKey\n  name: Custom Header Authentication\n  evidence: Custom headers add authentication data to API requests via HTTP headers. Common implementations include API keys and bearer tokens.\n  how_to_obtain: Configure a header name (e.g., \"Authorization\" or \"X-API-Key\") and a static or dynamic header value in the API connection settings.\n\
  - type: other\n  name: Android SDK – Request Context Provider\n  evidence: The request context provider is a function that returns a map with keys and values agreed upon with ASAPP.\n  how_to_obtain: Implement ASAPPRequestContextProvider that returns an Auth map containing a Token.\ndocs: https://docs.asapp.com/generativeagent/integrate/web-sdk/web-authentication.md\nnote: 4 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/asapp3/refs/heads/main/authentication/asapp3-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- Customer Experience
- Enterprise
- Contact Center
- Platform
- Company
---
