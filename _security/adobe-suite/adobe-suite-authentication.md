---
api_key_in:
- cookie
- header
- query
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Adobe Photoshop API
  slug: adobe-photoshop-api
  spec_type: OpenAPI
  url: https://developer.adobe.com/photoshop/api/openapi/
- filename: openapi.yaml
  format: yaml
  label: Adobe Lightroom API
  slug: adobe-lightroom-api
  spec_type: OpenAPI
  url: https://developer.adobe.com/lightroom/api/openapi/
- filename: adobe-suite-firefly-illustrator-openapi.json
  format: json
  label: Adobe Illustrator API
  slug: adobe-illustrator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-suite/refs/heads/main/openapi/adobe-suite-firefly-illustrator-openapi.json
- filename: adobe-suite-firefly-indesign-openapi.json
  format: json
  label: Adobe InDesign API
  slug: adobe-indesign-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-suite/refs/heads/main/openapi/adobe-suite-firefly-indesign-openapi.json
- filename: openapi.yaml
  format: yaml
  label: Adobe PDF Services API
  slug: adobe-pdf-services-api
  spec_type: OpenAPI
  url: https://developer.adobe.com/document-services/docs/apis/
- filename: openapi.yaml
  format: yaml
  label: Adobe PDF Extract API
  slug: adobe-pdf-extract-api
  spec_type: OpenAPI
  url: https://developer.adobe.com/document-services/docs/apis/
- filename: openapi.yaml
  format: yaml
  label: Adobe PDF Accessibility Auto-Tag API
  slug: adobe-pdf-accessibility-auto-tag-api
  spec_type: OpenAPI
  url: https://developer.adobe.com/document-services/docs/apis/
- filename: adobe-suite-analytics-openapi.json
  format: json
  label: Adobe Analytics API
  slug: adobe-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-suite/refs/heads/main/openapi/adobe-suite-analytics-openapi.json
- filename: adobe-suite-firefly-openapi.json
  format: json
  label: Adobe Firefly API
  slug: adobe-firefly-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-suite/refs/heads/main/openapi/adobe-suite-firefly-openapi.json
- filename: adobe-suite-firefly-audio-video-openapi.json
  format: json
  label: Adobe Firefly Audio/Video APIs
  slug: adobe-firefly-audiovideo-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-suite/refs/heads/main/openapi/adobe-suite-firefly-audio-video-openapi.json
- filename: adobe-suite-cc-libraries-openapi.json
  format: json
  label: Adobe Creative Cloud Libraries API
  slug: adobe-creative-cloud-libraries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-suite/refs/heads/main/openapi/adobe-suite-cc-libraries-openapi.json
- filename: adobe-suite-firefly-express-openapi.json
  format: json
  label: Adobe Express Embed SDK
  slug: adobe-express-embed-sdk
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-suite/refs/heads/main/openapi/adobe-suite-firefly-express-openapi.json
- filename: adobe-suite-aep-schema-registry-openapi.yaml
  format: yaml
  label: Adobe Experience Platform API
  slug: adobe-experience-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-suite/refs/heads/main/openapi/adobe-suite-aep-schema-registry-openapi.yaml
- filename: adobe-suite-marketo-identity-openapi.json
  format: json
  label: Adobe Marketo Engage API
  slug: adobe-marketo-engage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-suite/refs/heads/main/openapi/adobe-suite-marketo-identity-openapi.json
- filename: adobe-suite-commerce-rest-guest-openapi.yaml
  format: yaml
  label: Adobe Commerce API
  slug: adobe-commerce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-suite/refs/heads/main/openapi/adobe-suite-commerce-rest-guest-openapi.yaml
- filename: adobe-suite-cloud-manager-openapi.yaml
  format: yaml
  label: Adobe Cloud Manager API
  slug: adobe-cloud-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-suite/refs/heads/main/openapi/adobe-suite-cloud-manager-openapi.yaml
- filename: adobe-suite-journey-optimizer-campaigns-retrieve-openapi.yaml
  format: yaml
  label: Adobe Journey Optimizer API
  slug: adobe-journey-optimizer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-suite/refs/heads/main/openapi/adobe-suite-journey-optimizer-campaigns-retrieve-openapi.yaml
- filename: adobe-suite-workfront-workflow-openapi.json
  format: json
  label: Adobe Workfront API
  slug: adobe-workfront-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-suite/refs/heads/main/openapi/adobe-suite-workfront-workflow-openapi.json
- filename: adobe-suite-firefly-substance-3d-openapi.yaml
  format: yaml
  label: Adobe Substance 3D API
  slug: adobe-substance-3d-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-suite/refs/heads/main/openapi/adobe-suite-firefly-substance-3d-openapi.yaml
- filename: adobe-suite-data-collection-openapi.yaml
  format: yaml
  label: Adobe Experience Platform Edge Network API
  slug: adobe-experience-platform-edge-network-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-suite/refs/heads/main/openapi/adobe-suite-data-collection-openapi.yaml
- filename: adobe-suite-status-openapi.yaml
  format: yaml
  label: Adobe Status API
  slug: adobe-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-suite/refs/heads/main/openapi/adobe-suite-status-openapi.yaml
- filename: adobe-suite-vip-marketplace-partners-openapi.json
  format: json
  label: Adobe VIP Marketplace Partner API
  slug: adobe-vip-marketplace-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-suite/refs/heads/main/openapi/adobe-suite-vip-marketplace-partners-openapi.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Adobe Suite Authentication
name_suffix: Authentication
oauth_flows: []
overview: Adobe Suite secures its APIs with apiKey and http across 12 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Adobe Suite
provider_slug: adobe-suite
scheme_count: 12
schemes:
- in: header
  name: api_key
  parameter: api_key
  sources:
  - openapi/adobe-suite-commerce-rest-customer-openapi.yaml
  - openapi/adobe-suite-commerce-rest-guest-openapi.yaml
  type: apiKey
- description: API Access Key
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/adobe-suite-data-collection-openapi.yaml
  - openapi/adobe-suite-firefly-audio-video-openapi.json
  - openapi/adobe-suite-firefly-illustrator-openapi.json
  - openapi/adobe-suite-firefly-indesign-openapi.json
  - openapi/adobe-suite-firefly-lightroom-openapi.json
  - openapi/adobe-suite-firefly-openapi.json
  - openapi/adobe-suite-firefly-substance-3d-openapi.yaml
  - openapi/adobe-suite-firefly-translate-lipsync-openapi.json
  - openapi/adobe-suite-journey-optimizer-campaigns-retrieve-openapi.yaml
  - openapi/adobe-suite-vip-marketplace-partners-openapi.json
  type: apiKey
- bearerFormat: JWT
  description: Should be a valid IMS token for authenticating with the Edge Gateway
  name: IMSAuth
  scheme: bearer
  sources:
  - openapi/adobe-suite-data-collection-openapi.yaml
  - openapi/adobe-suite-firefly-audio-video-openapi.json
  - openapi/adobe-suite-firefly-express-openapi.json
  - openapi/adobe-suite-firefly-illustrator-openapi.json
  - openapi/adobe-suite-firefly-indesign-openapi.json
  - openapi/adobe-suite-firefly-lightroom-openapi.json
  - openapi/adobe-suite-firefly-openapi.json
  - openapi/adobe-suite-firefly-substance-3d-openapi.yaml
  - openapi/adobe-suite-firefly-translate-lipsync-openapi.json
  - openapi/adobe-suite-firefly-workflow-builder-openapi.yaml
  - openapi/adobe-suite-journey-optimizer-content-openapi.yaml
  - openapi/adobe-suite-journey-optimizer-journey-retrieve-openapi.yaml
  - openapi/adobe-suite-journey-optimizer-messaging-openapi.yaml
  - openapi/adobe-suite-journey-optimizer-orchestrated-campaign-dataset-openapi.yaml
  - openapi/adobe-suite-journey-optimizer-simulations-openapi.yaml
  - openapi/adobe-suite-journey-optimizer-suppression-openapi.yaml
  - openapi/adobe-suite-status-openapi.yaml
  - openapi/adobe-suite-workfront-unified-approvals-openapi.json
  type: http
- in: header
  name: apiKey
  parameter: X-API-KEY
  sources:
  - openapi/adobe-suite-firefly-express-openapi.json
  type: apiKey
- description: User access token (Bearer xxx)
  name: Authorization
  scheme: Bearer
  sources:
  - openapi/adobe-suite-firefly-photoshop-v2-openapi.json
  type: http
- description: Api key (adobe.io)
  in: header
  name: X-Api-Key
  parameter: X-Api-Key
  sources:
  - openapi/adobe-suite-firefly-photoshop-v2-openapi.json
  type: apiKey
- description: Use the api key `StatusAdobeIOClient`
  in: query
  name: api_key
  parameter: api_key
  sources:
  - openapi/adobe-suite-status-openapi.yaml
  type: apiKey
- in: header
  name: authorization
  parameter: authorization
  sources:
  - openapi/adobe-suite-vip-marketplace-partners-openapi.json
  type: apiKey
- in: header
  name: SessionIDHeader
  parameter: sessionID
  sources:
  - openapi/adobe-suite-workfront-workflow-openapi.json
  type: apiKey
- in: cookie
  name: AtTaskCookie
  parameter: attask
  sources:
  - openapi/adobe-suite-workfront-workflow-openapi.json
  type: apiKey
- in: cookie
  name: WFAuthCookie
  parameter: wf-auth
  sources:
  - openapi/adobe-suite-workfront-workflow-openapi.json
  type: apiKey
- in: header
  name: ApiKeyHeader
  parameter: apiKey
  sources:
  - openapi/adobe-suite-workfront-workflow-openapi.json
  type: apiKey
slug: adobe-suite-authentication
source_filename: adobe-suite-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/ (70 documents) + https://developer.adobe.com/developer-console/docs/guides/authentication/\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\n  - header\n  - query\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: api_key\n  sources:\n  - openapi/adobe-suite-commerce-rest-customer-openapi.yaml\n  - openapi/adobe-suite-commerce-rest-guest-openapi.yaml\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: API Access Key\n  sources:\n  - openapi/adobe-suite-data-collection-openapi.yaml\n  - openapi/adobe-suite-firefly-audio-video-openapi.json\n  - openapi/adobe-suite-firefly-illustrator-openapi.json\n  - openapi/adobe-suite-firefly-indesign-openapi.json\n  - openapi/adobe-suite-firefly-lightroom-openapi.json\n  - openapi/adobe-suite-firefly-openapi.json\n  - openapi/adobe-suite-firefly-substance-3d-openapi.yaml\n  - openapi/adobe-suite-firefly-translate-lipsync-openapi.json\n\
  \  - openapi/adobe-suite-journey-optimizer-campaigns-retrieve-openapi.yaml\n  - openapi/adobe-suite-vip-marketplace-partners-openapi.json\n- name: IMSAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Should be a valid IMS token for authenticating with the Edge Gateway\n  sources:\n  - openapi/adobe-suite-data-collection-openapi.yaml\n  - openapi/adobe-suite-firefly-audio-video-openapi.json\n  - openapi/adobe-suite-firefly-express-openapi.json\n  - openapi/adobe-suite-firefly-illustrator-openapi.json\n  - openapi/adobe-suite-firefly-indesign-openapi.json\n  - openapi/adobe-suite-firefly-lightroom-openapi.json\n  - openapi/adobe-suite-firefly-openapi.json\n  - openapi/adobe-suite-firefly-substance-3d-openapi.yaml\n  - openapi/adobe-suite-firefly-translate-lipsync-openapi.json\n  - openapi/adobe-suite-firefly-workflow-builder-openapi.yaml\n  - openapi/adobe-suite-journey-optimizer-content-openapi.yaml\n  - openapi/adobe-suite-journey-optimizer-journey-retrieve-openapi.yaml\n\
  \  - openapi/adobe-suite-journey-optimizer-messaging-openapi.yaml\n  - openapi/adobe-suite-journey-optimizer-orchestrated-campaign-dataset-openapi.yaml\n  - openapi/adobe-suite-journey-optimizer-simulations-openapi.yaml\n  - openapi/adobe-suite-journey-optimizer-suppression-openapi.yaml\n  - openapi/adobe-suite-status-openapi.yaml\n  - openapi/adobe-suite-workfront-unified-approvals-openapi.json\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  sources:\n  - openapi/adobe-suite-firefly-express-openapi.json\n- name: Authorization\n  type: http\n  scheme: Bearer\n  description: User access token (Bearer xxx)\n  sources:\n  - openapi/adobe-suite-firefly-photoshop-v2-openapi.json\n- name: X-Api-Key\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  description: Api key (adobe.io)\n  sources:\n  - openapi/adobe-suite-firefly-photoshop-v2-openapi.json\n- name: api_key\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: Use the api key `StatusAdobeIOClient`\n\
  \  sources:\n  - openapi/adobe-suite-status-openapi.yaml\n- name: authorization\n  type: apiKey\n  in: header\n  parameter: authorization\n  sources:\n  - openapi/adobe-suite-vip-marketplace-partners-openapi.json\n- name: SessionIDHeader\n  type: apiKey\n  in: header\n  parameter: sessionID\n  sources:\n  - openapi/adobe-suite-workfront-workflow-openapi.json\n- name: AtTaskCookie\n  type: apiKey\n  in: cookie\n  parameter: attask\n  sources:\n  - openapi/adobe-suite-workfront-workflow-openapi.json\n- name: WFAuthCookie\n  type: apiKey\n  in: cookie\n  parameter: wf-auth\n  sources:\n  - openapi/adobe-suite-workfront-workflow-openapi.json\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: apiKey\n  sources:\n  - openapi/adobe-suite-workfront-workflow-openapi.json\ndocs: https://developer.adobe.com/developer-console/docs/guides/authentication/\nnote: 'Derived mechanically from all 70 harvested OpenAPI documents, then upgraded from Adobe''s own authentication\n  documentation.\
  \ IMPORTANT: the specs under-report reality. Every Adobe spec models auth as an apiKey header plus\n  an HTTP bearer token, but the bearer token is in fact an Adobe IMS OAuth 2.0 access token minted at https://ims-na1.adobelogin.com/ims/token/v3\n  with an explicit scope list. No spec declares an oauth2 securityScheme, so an agent reading the contract alone\n  cannot discover the authorization server, the grant, the scopes or the 24-hour token lifetime. See scopes/adobe-suite-scopes.yml\n  and well-known/adobe-suite-openid-configuration.json.'\ncredential_types:\n- name: OAuth Server-to-Server\n  grant: client_credentials\n  status: current\n  docs: https://developer.adobe.com/developer-console/docs/guides/authentication/ServerToServerAuthentication/\n  note: Replaced the deprecated JWT (Service Account) credential, retired 2025-06-30.\n- name: OAuth Web App\n  grant: authorization_code\n  status: current\n- name: OAuth Single Page App\n  grant: authorization_code + PKCE\n  status: current\n\
  - name: OAuth Native App\n  grant: authorization_code + PKCE\n  status: current\n- name: API Key credential\n  grant: none (client-side key only)\n  status: current\n  note: Used by client-side surfaces such as the Adobe Express Embed SDK and PDF Embed API.\n- name: JWT / Service Account\n  grant: urn:ietf:params:oauth:grant-type:jwt-bearer\n  status: deprecated\n  retired: '2025-06-30'\n  docs: https://developer.adobe.com/developer-console/docs/guides/authentication/JWT/\ntransport_headers:\n- header: Authorization\n  value: Bearer <IMS access token>\n  required: true\n  occurrences_in_specs: 1494\n- header: x-api-key\n  value: <Client ID from Adobe Developer Console>\n  required: true\n  occurrences_in_specs: 2326\n- header: x-gw-ims-org-id\n  value: <IMS Org ID>\n  required: per-service\n  occurrences_in_specs: 1660\n  note: Required by every Experience Cloud API (Experience Platform, Journey Optimizer, Marketo MCP). This is the\n    tenancy selector.\ntoken:\n  lifetime: 24 hours\n\
  \  refresh: re-issue via client_credentials; refresh_token supported on user flows\n  endpoint: https://ims-na1.adobelogin.com/ims/token/v3\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adobe-suite/refs/heads/main/authentication/adobe-suite-authentication.yml
summary_line: apiKey/http · 12 schemes
tags:
- Ai
- Analytics
- Automation
- Commerce
- Creative
- Design
- Documents
- Experience
- Marketing
- Personalization
- Video
---
