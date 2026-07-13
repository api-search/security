---
api_key_in: []
api_specs:
- filename: adobe-experience-manager-openapi.yml
  format: yaml
  label: Adobe Experience Manager APIs
  slug: apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-experience-manager/refs/heads/main/openapi/adobe-experience-manager-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Adobe Experience Manager Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Adobe Experience Manager secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Adobe Experience Manager
provider_slug: adobe-experience-manager
scheme_count: 1
schemes:
- description: Adobe IMS OAuth 2.0 with Server-to-Server credentials issued from the Adobe Developer Console for an AEM as a Cloud Service project.
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://ims-na1.adobelogin.com/ims/token/v3
  name: adobeIMS
  sources:
  - openapi/adobe-experience-manager-openapi.yml
  type: oauth2
slug: adobe-experience-manager-authentication
source_filename: adobe-experience-manager-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/adobe-experience-manager-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: adobeIMS\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://ims-na1.adobelogin.com/ims/token/v3\n    scopes: 0\n  description: Adobe IMS OAuth 2.0 with Server-to-Server credentials issued from the Adobe Developer\n    Console for an AEM as a Cloud Service project.\n  sources:\n  - openapi/adobe-experience-manager-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adobe-experience-manager/refs/heads/main/authentication/adobe-experience-manager-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Content Management
- Enterprise CMS
- Digital Asset Management
- Headless CMS
- Content Fragments
- Adaptive Forms
---
